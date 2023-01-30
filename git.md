---
title: "Git"
date: 2023-01-24T04:35:00-04:00
tags: [Raspberry Pi, Git, apt-get install]
---
To work with a [Git](https://git-scm.com/) code repository, such as [GitHub](https://github.com/), the Git client application is one of the main tools to fascilitate the code movement and commands required to manage the repository.

## Prerequisites

- RPI
- [Raspberry Pi Operating System (OS) setup]( {{< relref "how-to/raspberry-pi/operating-system" >}})

## Steps

1. Login to the RPI.
1. Add Git repository.

   > **_Note:_** This is only required for the more recent version of Git.  If the older version would be fine, skip to step 4.

   ```
   sudo add-apt-repository ppa:git-core/ppa
   ```

1. Update repositories.

   ```
   sudo apt-get update
   ```

1. Setup Git.

   ```
   sudo apt-get install git
   ```

## References

- [The Odin Project: Install Git](https://www.theodinproject.com/lessons/foundations-setting-up-git#step-1-install-git)