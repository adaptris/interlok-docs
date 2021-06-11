# JDBC Statement Builder

The statement builder (both capture and query) aims to simplify the
syntax when writing SQL statements. Part of its goals are to make
statement-parameters redundant and thus we needed a new syntax.

## Syntax

The syntax for the statement builder is made up of three parts: *from*,
*what*, and *to*. Data can come from the following sources:

 * payload
 * metadata
 * xpath
 * constant
 * id

And forms the beginning of the resolvable expression: `%sql_payload` or
`%sql_id`, etc. For more information see:
`StatementParameterImpl.QueryType`.

The first component within the braces is the expected JDBC data type.
The available types come from the implementations of
`TypedStatementParameter` and are as follows:

 * STRING
 * SHORT
 * INTEGER
 * LONG
 * FLOAT
 * DOUBLE
 * BOOLEAN
 * DATE
 * TIME
 * TIMESTAMP

The second part within the braces, and final part overall, is the named
parameter reference---it can be whatever the user feels is suitable and
completes the resolvable statement builder expression:

    %sql_metadata{integer:a_primary_key}
    %sql_payload{string:some_column}
    %sql_id{string:message_id}
    %sql_metadata{timestamp:last_updated}

See `NamedParameterApplicator` for further information on using named
parameters in Interlok.

## Example

A detailed example of new config and how it relates to the old config.

```xml
<jdbc-data-capture-statement-builder-service>
  <unique-id>capture</unique-id>
  <connection class="shared-connection">
    <lookup-name>jdbc-connection</lookup-name>
  </connection>
  <statement>INSERT INTO file (id, name, size, data) VALUES
      (%sql_id{string:message_id}, %sql_metadata{string:originalName}, %sql_metadata{integer:fsFileSize},  %sql_payload{string:data})</statement>
</jdbc-data-capture-statement-builder-service>
```

Where under the covers we actually turn that into:

```xml
<jdbc-raw-data-capture-service>
  <unique-id>raw-capture</unique-id>
  <connection class="shared-connection">
    <lookup-name>jdbc-connection</lookup-name>
  </connection>
  <jdbc-string-statement-parameter>
    <name>message_id</name>
    <query-string>message_id</query-string>
    <query-type>id</query-type>
  </jdbc-string-statement-parameter>
  <jdbc-string-statement-parameter>
    <name>originalName</name>
    <query-string>originalName</query-string>
    <query-type>metadata</query-type>
  </jdbc-string-statement-parameter>
  <jdbc-integer-statement-parameter>
    <name>fsFileSize</name>
    <query-string>fsFileSize</query-string>
    <query-type>metadata</query-type>
  </jdbc-integer-statement-parameter>
  <jdbc-string-statement-parameter>
    <name>data</name>
    <query-string>data</query-string>
    <query-type>payload</query-type>
  </jdbc-string-statement-parameter>
  <statement>INSERT INTO file (id, name, size, data) VALUES
             (#id, #originalName, #fsFileSize,  #data)</statement>
</jdbc-raw-data-capture-service>
```
