---
title: "ssh-keygen -t ed25519 -f <filename> -C <email-address>"
date: 2023-02-04T10:25:00-04:00
tags: [ssh-keygen]
---
Generates a public/private key pair with the Ed25519 digital signature with the naming specified for the file (this allows multiple keys to be generated on the same computer).  Includes the email address in the encoding.

*Note: The inclusion of the email address is preferred for the usage with [GitHub](https://github.com/)