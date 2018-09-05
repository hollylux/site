# How to generate CSR

## What

When we want to enable https for a web site, we need to get a certificate from [CA](https://en.wikipedia.org/wiki/Certificate_authority). In order to get a certificate, we need to generate a [CSR](https://en.wikipedia.org/wiki/Certificate_signing_request), and send it to CA who will issue a new certificate to us.

## How

Here is an example of generating a CSR by using openssl:

```bash
openssl req -new -newkey rsa:2048 -nodes -keyout server.key -out server.csr
```

## Ref

[https://www.jamf.com/jamf-nation/articles/115/enabling-ssl-on-tomcat-with-a-public-certificate](https://www.jamf.com/jamf-nation/articles/115/enabling-ssl-on-tomcat-with-a-public-certificate)

