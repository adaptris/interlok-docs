> **Summary:** The JSON Web Token set of services allows Interlok to create, encode and decode JWTs

JSON Web Tokens (JWTs) are a compact, URL-safe means of representing claims to be transferred between parties. JWTs can be used as a way of securely transmitting information between different systems, and they are commonly used in web applications as a means of authentication and authorization. Interlok has a set of services for creating, decoding and encoding JWTs. For example, you might wish to generate a JWT and pass it along as a header in a HTTP request, or you might wish to decode an incoming JWT and extract the JSON object.

The three services are [jwt-creator][], [jwt-decode][] and [jwt-encode][]

## JWT Creator ##
```xml
   <jwt-creator>
      <unique-id>jwt-create</unique-id>
      <issuer>ashley</issuer>
      <subject>test</subject>
      <audience>everyone</audience>
      <expiration>2040-12-31 00:00:00.0 UTC</expiration>
      <not-before>2020-01-01 00:00:00.0 UTC</not-before>
      <secret class="base64-encoded-secret">
        <secret>c64975ba3cf3f9cd58459710b0a42369f34b0759c9967fb5a47eea488e8bea79</secret>
        <algorithm>HS256</algorithm>
      </secret>
      <custom-claims>
        <key-value-pair>
          <key>payload</key>
          <value>%message{%payload}</value>
        </key-value-pair>
      </custom-claims>
    </jwt-creator>
```
- Creates a JWT using key/value pairs.
- Signs the JWT with either a secret(using the HMAC algorithm), a public/private key pair(using RSA) or a PGP key.
- The JWT is then set as the current payload.

## JWT Decode ##
```xml
   <jwt-decode>
      <unique-id>jwt-decode</unique-id>
      <jwt-string class="string-payload-data-input-parameter"/>
      <secret class="base64-encoded-secret">
        <secret>c64975ba3cf3f9cd58459710b0a42369f34b0759c9967fb5a47eea488e8bea79</secret>
        <algorithm>HS256</algorithm>
      </secret>
      <header class="multi-payload-string-output-parameter">
        <payload-id>header</payload-id>
      </header>
      <claims class="multi-payload-string-output-parameter">
        <payload-id>claims</payload-id>
      </claims>
    </jwt-decode>
```
- Takes a JWT and allows you to decode it to extract the JSON object.
- Decodes the JWT with either a secret(using the HMAC algoithm), a public/private key pair(using RSA) or a PGP key.

## JWT Encode ##
```xml
   <jwt-encode>
      <unique-id>jwt-encode</unique-id>
      <header class="multi-payload-string-input-parameter">
        <payload-id>header</payload-id>
      </header>
      <claims class="multi-payload-string-input-parameter">
        <payload-id>claims</payload-id>
      </claims>
      <secret class="base64-encoded-secret">
        <secret>c64975ba3cf3f9cd58459710b0a42369f34b0759c9967fb5a47eea488e8bea79</secret>
        <algorithm>HS256</algorithm>
      </secret>
      <jwt-output class="multi-payload-string-output-parameter">
        <payload-id>output</payload-id>
      </jwt-output>
    </jwt-encode>
```
- Creates a JWT using inputted data.
- Signs the JWT with either a secret(using the HMAC algorithm), a public/private key pair(using RSA) or a PGP key.
- The JWT can then be output as either the current payload, as metadata, etc

?> When defining what type of encoded secret you wish to you if you are using the base64 or rsa options you can define which algorithm you wish to use(i.e HS256, HS384, RS256, RS384).

## Further Reading ##

More information around JWTs can be found here:

[JWT Introduction][]


[jwt-creator]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-json-web-token/4.7-SNAPSHOT/com/adaptris/core/jwt/JWTCreator.html
[jwt-decode]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-json-web-token/4.7-SNAPSHOT/com/adaptris/core/jwt/JWTDecoder.html
[jwt-encode]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-json-web-token/4.7-SNAPSHOT/com/adaptris/core/jwt/JWTEncoder.html
[JWT Introduction]: https://jwt.io/introduction