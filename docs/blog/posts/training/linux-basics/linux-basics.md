---
date: 2023-09-20
categories:
  - Training
authors:
  - silk
slug: linux-basics
draft: true
---

# Linux Basics

Now that you have a Linux virtual machine set up, let's get cooking on the command-line.

![Linux Terminal](./images/whoami.png)

<!-- more -->

[*Haven't set up a virtual machine yet? Click me!*](../setting-up-kali/setting-up-kali.md)

## Why?

Linux is used everywhere in the field of cybersecurity. Why? Because it's useful. Its usefulness has led to a thriving ecosystem of people and software. This is why so many of the tools we will use have been developed for Linux, and why we continue to use it.

## Overview

A quick reference guide and overview of the Linux filesystem.


## In-depth

### Users


### Commands


### File System

Links

## Cheatsheet

### Commands

| Command   | Description                     | Examples                                                          |
| --------- | ------------------------------- | ----------------------------------------------------------------- |
| `man`     | view manual for a command       | `man ls`                                                          |
| `ls`      | list directory contents         | `ls`, `ls -la`                                                    |
| `cd`      | change directory                | `cd my_dir`, `cd ..`, `cd /`                                      |
| `mkdir`   | make a directory                | `mkdir my_dir`, `mkdir -p my_dir/sub_dir`                         |
| `echo`    | print a line of text            | `echo hello world`, <br/> `echo hello world > my_file`            |
| `touch`   | create a file with no contents  | `touch my_file`                                                   |
| `cat`     | print a file's contents         | `cat my_file`                                                     |
| `grep`    | print lines that match patterns | `grep my_pattern my_file`, <br/> `some_command | grep my_pattern` |
| `find`    | find files based on criteria    | `find . -name my_file`                                            |
| `pwd`     | print path of current directory | `pwd`                                                             |
| `whoami`  | print current username          | `whoami`                                                          |
| `nano`    | open text editor                | `nano my_file`                                                    |
| `strings` | print human-readable strings    | `strings my_file`                                                 |
| `wget`    | file downloader                 | `wget unbcybersec.com`, <br/> `wget unbcybersec.com -O dest_file.html`                                                                  |
### File System

| Directory  | Description                                                                              |
| ---------- | ---------------------------------------------------------------------------------------- |
| `.`        | current directory                                                                        |
| `..`       | parent directory                                                                         |
| `/`        | root directory                                                                           |
| `~`        | home directory (of the current user)                                                     |
| `/home`    | contains home directories of users                                                       |
| `/root`    | root user's home directory                                                               |
| `/tmp`     | contains temporary files/directories                                                     |
| `/etc`     | configuration files and system-wide settings for various programs                        |
| `/var`     | contains 'variable' data, often logs, saved data for services, etc.                      |
| `/run`     | contains various runtime files managed by the system, such as process IDs, sockets, etc. |
| `/srv`     | contains data used services, often web services (web page files)                         |
| `/sys`     | provides files for configuring kernel parameters and hardware devices                    |
| `/dev`     | contains special files representing hardware devices                                     |
| `/mnt`     | used to mount devices, partitions, and network shares                                    |
| `/media`   | external media devices are often mounted here                                            |
| `/bin`     | contains binary executables                                                              |
| `/usr/bin` | also contains binary executables, usually `/bin` is linked to here                       |
| `/sbin`    | contains system binary executables                                                       |
| `/lib`     | contains shared libraries                                                                |
| `/opt`     | provides a standard location for optionally installed software                           |

