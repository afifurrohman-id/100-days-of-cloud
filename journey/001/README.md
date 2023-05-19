# Virtualization & Linux Fundamental

## Introduction

The very first thing to learn about cloud technology is virtualization and get to know Linux more closely, The journey will be like this:

- Virtualization
- Linux Hierarchy Directory
- Linux Basic Command

## Cloud Research

### - Virtualization Concept

What is virtualization?<br>
Virtualization is the process of creating a virtual version of a computing environment, such as a server, operating system, or network resources

In this journey i learn about two virtualization type, here for example:

#### 1. Virtual Machine

This type of virtualization creates a separate operating system environment within a host operating system, allowing multiple operating systems to run on a single physical device.
![vType1](https://user-images.githubusercontent.com/118882411/210575921-8a9f20f4-c145-45e7-946f-f8342a63af29.jpg)

#### 2. Hardware Virtualization

This type of virtualization allows a physical device to be divided into multiple virtual devices, each with its own operating system and resources.
![VType2](https://user-images.githubusercontent.com/118882411/210580141-4d7720f4-6077-4a28-9dad-6c52e39372e8.jpg)

### Linux Hierarchy Directory

The Linux hierarchy directory is structure of directory in linux, for example view my graphic:
![linuxHierarchyDirectory](https://user-images.githubusercontent.com/118882411/210581840-64c2c49e-d3e6-4858-b78c-112e94aeee65.jpg)

#### Directory function

- /: The root directory is the top-level directory in the file system and contains all other directories and files on the system.

- /bin: /bin is binary, This directory contains essential command-line utilities and programs that are necessary for the system to function, for example like command <code>cd</code>, <code>mv</code>, <code>ls</code> etc..

- /sbin: Same like /bin, this directory contains system utilities and programs that are used for system maintenance and administration(Root).

- /etc: This directory contains system configuration files and scripts.

- /usr: This directory contains user-level programs and data, including libraries, documentation, and other resources.

- /var: /var is variable, This directory contains files that are expected to change during the normal operation of the system, such as logs, spool files, and temporary files.

- /tmp: /tmp is temporary, This directory contains temporary files that are created by the system or users. These files are typically deleted when the system is rebooted.

- /home: This directory contains the home directories for individual users, where they can store their personal files and documents.

- /dev: /dev is Device, This directory contains device files that represent devices such as printers, keyboards, and disk drives.

- /proc: /proc is peocess, This directory contains virtual files that provide information about the system's hardware and processes.

And etc..

### Linux Basic Command

This is the basic and most frequently used command:

<p>Note: For view help or show more option in command use <code>--help</code> option. For example <code>ls --help</code></p>

- <code>cd</code>: cd is Change Directory, use to change other directory
- <code>ls</code>: ls is List, use to view content in directory
- <code>mkdir</code>: mkdir is make directory, use to make directory
- <code>rm</code>: ls is remove, use to remove files or directory
- <code>rmdir</code>: ls is remove directory, use to remove empty directory
- <code>clear</code>: use to clear all text in terminal
- <code>history</code>: use to view history of command
- <code>cp</code>: cp is copy, use to copy file or directory
- <code>mv</code>: mv is move, use to move or rename file / directory

## Next Steps

✍️ Describe what you think you think you want to do next.

