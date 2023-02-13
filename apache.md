---
title: "Apache2"
date: 2023-01-24T04:28:00-04:i00
tags: [Raspberry Pi, Apache, apt-get install]
---
To host a web site on the Raspberry Pi (RPI), the system can be setup with the [Apache web server](https://httpd.apache.org/).

## Prerequisites

- RPI
- [Raspberry Pi Operating System (OS) setup]( {{< relref "how-to/raspberry-pi/operating-system" >}})

## Steps

1. Install Apache web server.

   ```
   sudo apt-get install apache2
   ```

1. Give `pi` user ownership of `/var/www` folder.

   ```
   sudo chown -R pi:www-data /var/www
   ```

1. Set user and group permissions.

   ```
   sudo chmod u+rxw,g+rx-w,o-rwx /var/www
   ```

1. Set new files created to belong to `www-data` group.

   ```
   sudo chmod g+s /var/www
   ```

## Optional

If there are existing files/folders, the following commands will update permissions.

For a file:

```
chmod u+rw,g+r-xw,o-rwx
```

For a directory:

```
chmod u+rwx,g+rx-w,o-rxw
```

## References

- [Raspberry Pi Forum: /var/www/html permissions](https://forums.raspberrypi.com/viewtopic.php?t=155067)