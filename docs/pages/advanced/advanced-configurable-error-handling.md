> **Summary:** This document describes the configurable error handling component within Interlok.

If the standard [`Error Handling`](../user-guide/adapter-error-handling.md) within Interlok does not provide the necessary functionality, you may use the `ConfigurableExceptionHandler` component.

## Configurable Error Handling

The `ConfigurableExceptionHandler` is a flexible and configurable component for handling exceptions. 
It allows developers to define rules for matching exceptions and execute specific services based on those rules. 
If no rules match, a default service can be executed as a fallback. This component is part of Interlok Core.

## Key Features

- **Rule-Based Exception Handling**: Match exceptions using regular expressions and handle them with specific services or a service list.
- **Field Matching**: Supports matching against exception fields such as:
    - Exception type
    - Exception message
    - Exception cause
    - Stack trace
- **Default Fallback Service**: Executes a default service if no rules match.

## Fields

**Processing Exception Service**: Chose a service to handle exceptions when no rules match.

**Rules**: A list of rules for matching exceptions and executing corresponding services.

### Nested Fields

**Exception Rule**: Represents a rule for handling specific exceptions. A rule contains a `Matcher` with a `Regular Expression` field to match 
  against either:
  - Exception
  - Exception Cause
  - Exception Message
  - Stack Trace

A Rule also contains a `Processing Exception Service` to execute if the rule matches. This could also be a Service List.

## Usage Example

The below example shows a `ConfigurableExceptionHandler` that has a Rule and default fallback service defined.
The default service is shown first with a list of rules below as `<exception-rule>` objects. Each rule shows a `matcher`
and `processing-exception-service` as described above. 

!> **IMPORTANT** The rules will be evaluated in the order they are written. Only the first matched rule will process the exception.

### Configuration
```xml
<configurable-exception-handler>
    <unique-id>example-ConfigurableExceptionHandler</unique-id>
    <default-exception-processing-service class="log-message-service">
        <unique-id>default-service</unique-id>
        <log-level>DEBUG</log-level>
        <log-prefix>default-logger-</log-prefix>
        <logging-format class="message-logging-default"/>
    </default-exception-processing-service>
    <exception-rule>
        <matcher>
            <regex>.*error.*</regex>
            <match-against-field>EXCEPTION_MESSAGE</match-against-field>
        </matcher>
        <exception-processing-service class="log-message-service">
            <unique-id>rule-service</unique-id>
            <log-level>DEBUG</log-level>
            <log-prefix>matched-rule-logger-</log-prefix>
            <logging-format class="message-logging-with-payload"/>
        </exception-processing-service>
    </exception-rule>
</configurable-exception-handler>
```

## Core Concepts

- The default service is optional but highly recommended for fallback behavior.
- Rules are evaluated in the order they are added to the `rules` list.
- Only the first matched rule will process the exception or the default service if no rules are matched.

## See Also

- [`Error Handling`](../user-guide/adapter-error-handling.md)