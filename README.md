# IoT-Security

IoT Security in deep overview and details about the ceritifcates which were used in the IoT Security practises around the world and also about the multiple security levels
used currently to keep the devices safe and secure.

Topics

- Understanding Ceritificates
- MQTT Authetication Methods


## Understanding Certificates

Under the IoT Security there are totally 4 categories
- Confidentiality     - Encryption
- Trust               - Identity + Integity
- Non - Repudiation   - Trust + Contract/Legal
- Availablity         - Isolating Components

### Registration Authority

- Carries out checks on users to verify their identity using a specific process called the ***Certificate Practise Statement(CPS)***
- Follows the ***PKI ( Public Key Infrastructure)*** process used to **Issue,** **Validate,** **Manage,** and **Revoke** Certificates
- Can Generate the Public and Private Keypair if this is not done in a user ***PSE (Personal Secure Environment)***
- Instruct Certificate Authorities to issue Certificates.
- Examples: Let's Encrypt, Comodom, Symantec, DigiCert, GeoTrust


## TLS vs SSL

TLS and SSL both are protocols that helps you securely authenticate and transport data on the internet. 

### Difference Between TLS and SSL

- TLS stands for **Transport Layer Security** 
- SSL stands for **Secure Socket Layers**
- TLS and SSL both cryptographic protocols that encrypt data and authenticate a connection when data transferring on the internet
- Eg: banking and secure transcation
- TLS is more recent version of SSL, TLS fixes some security vulnerablities in the earlier SSL Protocols


### History Of SSL and TLS

- SSL 1.0 = Never publicly released due to security issues
- SSL 2.0 = released in 1995. Deprecated in 2011 (known security issues)
- SSL 3.0 = released in 1996. Deprecated in 2015 (known security issues)
- TLS 1.0 = released in 1999 as an upgrade to SSL 3.0. (deprecation in 2020)
- TLS 1.1 = released in 2006. (deprecation in 2020)
- TLS 1.2 = released in 2008
- TLS 1.3 = released in 2018

### TLS and SSL work to secure Data

<p align = "left">
     When you install an SSL/TLS certificate on your web server (often called as SSL certificate) it includes a public key and private key that authenticate server and let server encrypt and decrypt data
     
     when client goes on site, the web browser will look for client site's SSL/TLS ceritificate. Then the client browser will perform a handshake to check and validate of client certificate and autheticate.
     
     If the SSL Certificate is not valid, your client may be faces with "your connection is not private/secure" error, which could cause them not to connect the server and client may leave website
     
     if the client browser determines that certificate is valid and authenticates your server, it essentially creates an encrypted link between it and your server to securely transport data.
     
     This is also where HTTPS comes in (HTTPS stands HTTP over SSL/TLS)
     
     While Plain HTTP that information is vulnerable to attacks. But when you use HTTP over SSL or TLS (HTTPS) you encrypt and authenticate that data during transport which makes it secure.
     
     This is why we can safely process money transactions details over HTTPS but not over HTTP.
     </p>
     
### Why SSL still holds on?
<p align = "left">
     
     TLS is the more recent version of SSL and that both public released of SSL have been deprecated for multiple years and contain known security vulnerabilities.
     
     But still is it called an SSL ceritificate and not a TLS ceritificate, reason why most people still refer to them as SSL certificates is basically a branding issue. Most major certificate providers still refer to certificates as SSL certificates, which is why the naming convention persists.
     
     In reality all the SSL Certificates, that you see advertised are really ***SSL/TLS Certificates***
     We can use both SSL and TLS protocols with Single handled certificates
     There's no such thing as just an SSL Certificate or Just a TLS certificate and you don't need to worry about replacing Your SSL ceritifcates with a TLS Certificate
     </p>
     
**Note:** We can also Replace TLS instead of SSL with same certificate
