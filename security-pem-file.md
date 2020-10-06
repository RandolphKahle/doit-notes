---
date: 2020-10-06T09:48
tags:
  - security/
---

# security-pem-file

# PEM file

A remnant of the Privacy Enhanced Mail effort. This is the container format.

PEM - Governed by RFCs, its used preferentially by open-source software. It can have a variety of extensions:
* .pem, 
* .key, 
* .cer, 
* .cert, 
* more


.pem - Defined in RFCs [1421](https://tools.ietf.org/html/rfc1421) through [1424](https://tools.ietf.org/html/rfc1424), this is a container format that may include just the public certificate (such as with Apache installs, and CA certificate files /etc/ssl/certs), or may include an entire certificate chain including public key, private key, and root certificates. Confusingly, it may also encode a CSR (e.g. as used here) as the PKCS10 format can be translated into PEM. The name is from Privacy Enhanced Mail (PEM), a failed method for secure email but the container format it used lives on, and is a base64 translation of the x509 ASN.1 keys