---
title: "Setup"
date: 2023-01-24T04:35:00-04:00
tags: [Raspberry Pi, Git, apt-get install]
---
These are some setup configurations to help with the usage of Git.

## Prerequisites

- RPI
- [Raspberry Pi Operating System (OS) setup]( {{< relref "how-to/raspberry-pi/operating-system" >}})
- [Git install]( {{< relref "how-to/raspberry-pi/git/install" >}})

## Your Information

Identify to Git your information so that it identifies as you for actions that you perform.

```
git config --global user.name "<your name>"
git config --global user.email "<your email address>"
```

## Default Branch

Set the default branch to the commonly used "main" naming convention.

```
git config --global init.defaultBranch main
```

## Colour Output

Set the output of Git to be coloured.

```
git config --global color.ui auto
```

## Pre-Merging Behaviour (Optional)

Identify that Git should rebase prior to merging.

```
git config --global pull.rebase false
```

## References

- [The Odin Project: Install Git](https://www.theodinproject.com/lessons/foundations-setting-up-git#step-1-install-git)