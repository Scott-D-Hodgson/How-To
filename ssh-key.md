---
title: "SSH Keygen"
date: 2023-02-04T10:25:00-04:00
tags: [Raspberry Pi, ssh-keygen]
---
To perform various protected operations with the Raspberry Pi (RPI), othen it is needed to create a Secure Shell (SSH) key combination (public and private pair) in order to establish secure connections.  This may be used to interface with GitHub repositories as well as communications between machines.

## Prerequisites

- RPI
- [Raspberry Pi OS setup]( {{< relref "how-to/raspberry-pi/operating-system" >}})

## Command

Depending on the need, different variants of keys may be needed to be generated.

If only an SSH key is required the following command will generate a key for the local user in the home folder of `~/.ssh/`.

   ```
   ssh-keygen -t ed25519
   ```

When using with [GitHub](https://github.com), include the `-C` parameter to specify the email address for future interactions with repositories.

```
ssh-keygen -t ed25519 -C <email-address>
```

If the intended usage will be for the root user to leverage the key, such as in a `crontab` or `systemd` process, generate the key with the sudo command.

```
sudo ssh-keygen -t ed25519
```

