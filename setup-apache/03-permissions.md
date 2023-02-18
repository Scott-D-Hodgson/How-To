---
title: "Permissions"
date: 2023-01-24T04:28:00-04:i00
tags: [Apache, chown, chmod]
---
1. Give user account ownership of `/var/www` folder.

   ```
   sudo chown -R <username>:www-data /var/www
   ```

   *Note: Replace `<username>` with the username of the account that will manage the files of the web server.  In Raspberry Pi Operating System (OS), this would be the `pi` user.

1. Set user and group permissions.

   ```
   sudo chmod u+rxw,g+rx-w,o-rwx /var/www
   ```

1. Set new files created to belong to `www-data` group.

   ```
   sudo chmod g+s /var/www
   ```

1. Optional configurations

   If there are existing files/folders, the following commands will update permissions.

   For a file:

   ```
   chmod u+rw,g+r-xw,o-rwx
   ```

   For a directory:

   ```
   chmod u+rwx,g+rx-w,o-rxw
   ```

---
**Source:** [Raspberry Pi Forum: /var/www/html permissions](https://forums.raspberrypi.com/viewtopic.php?t=155067)