---
title: "chmod u+rxw,g+rx-w,o-rwx /var/www"
date: 2023-01-24T04:28:00-04:i00
tags: [chmod, folder:/var/www]
---
Changes the permissions on the `/var/www` folder.  Sets the permissions to the following:

- user: read, write, execute
- group: read, execute, but not write
- other: no read, write, or execute

*Note: Often used to setup the Apache web server to permit the `pi` user to be able to write content to the web site root `/var/www/html`.

---
**Source:** [Raspberry Pi Forum: /var/www/html permissions](https://forums.raspberrypi.com/viewtopic.php?t=155067)