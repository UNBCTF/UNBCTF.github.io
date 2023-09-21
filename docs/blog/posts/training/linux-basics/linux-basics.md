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
## Commands

Arguably, the most important part of Linux is the commands. Commands allow for quick and extensible usage of programs installed on the system.

There are commands for listing files, making web requests, editing users, shutting down the system, and this list goes on. Practically everything in Linux can be done using commands, as long as you have the correct commands installed, and permissions to do so.

### Hello World

First, open a terminal in your virtual machine. In Kali, you can do this by clicking the Terminal icon in the top-left of the desktop.

![Terminal Icon](./images/terminal_icon.png)
![Linux Terminal](./images/terminal.png)

We will start off by looking at the `echo` command. This command simply echoes the provided text back to the output. For example, `echo hello world` will simply print `hello world`.

![Hello World](./images/helloworld.png)

There are two parts to this command:

1. `echo`: The command itself.
2. `hello world`: The arguments/parameters passed to the command. In this case, the parameter is simply text we want to be printed.

What are parameters? They're important, so let's look further into them.
### More Parameters

Parameters allow us to tune what a command does. For example, the `ls` command lists the files and directories within the current directory.

Another important command is `ls`, which lists files and sub-directories in the current directory.

![ls output](./images/ls.png)

One parameter available for the `ls` command is `-a`. The `-a` parameter prints hidden files, which are files in Linux that start with a `.` character.

![ls hidden](./images/ls_hidden.png)

Another parameter for the `ls` command is `-l`, which prints one entry per line. The `-l` parameter also outputs the file permissions, file size, and last write date for reach file.

![ls list](./images/ls_list.png)

Commands usually allow multiple parameters, and we can combine the `-l` and `-a` parameters in this case: `ls -l -a`. When parameters start with a dash (`-`), they can often be combined into one as well: `ls -la` (this is not always the case).

How can we find these parameters and unlock the functionality of commands? There are two ways usually:



### More Commands



## Users


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

