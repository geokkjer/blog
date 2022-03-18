+++
title = "Red Hat Certified System Administrator"
date = 2022-03-18
updated = 2022-03-18
description = "RHCSA"
[taxonomies]
tags = ["Red Hat","RHCSA", "linux"]
+++

So I have decided to get certified, my picks are the Red Hat Certified System Administrator(RHCSA), the Red Hat Cetrified Engineer(RHCE) and the Certified Kubernetes Administrator(CKA).

Let's start from the beginning with the most fundamental one, the RHSCA. This cert ensures that the student knows how to preform basic Linux system admin tasks and some Red Hat specific stuff.

<!--more-->

### Introduction to Linux

Linux is a kernel, a monolithic kernel and not a micro kernel. It's purpose is to make computers hardware usable. An operating System is a kernel plus a userland, such as GNU(Gnu is not Unix). Is linux about [choice](http://www.islinuxaboutchoice.com/).
Linux kernel interacts directly with the hardware and provides low level services to upper layer components.
A Linux distibution is sometimes a curated(read: configured) collection of software that is bundeled on top of, and along side, a Linux kernel. Sometimes it is not curated but the delivered either as build scripts or binary packages from upstream, we call this a meta-distribution. The Linux kernel is one of the biggest software projects that has ever existed, this is often attributed to the adoption of the GNU(GPL v2) lisence, which forces people and companies to collaborate and contribute their changes back upstream to the Linux kernel. The originator, and still, main maintainer of Linux is Linux Thorvalds. Some notable fetures of the Linux kernel is that is sort of reimplementation of UNIX and it follows the POSIX standard. Everthing in Linux is a file, a for the most part the UNIX philosphy of one program that does one task very well is the standard. They(the kernel maintainers) also have a strrict rule of never breaking userland.

### Bootprocess

Booting -> bootloader -> linuk kernel -> pid1/systemd - userland

### Directories
Linux uses the [Filesystem Hierarchy Standars](https://refspecs.linuxfoundation.org/FHS_3.0/fhs/index.html)

>This standard consists of a set of requirements and guidelines for file and directory placement under UNIX-like operating systems. The guidelines are intended to support interoperability of applications, system administration tools, development tools, and scripts as well as greater uniformity of documentation for these systems.

```sh
tree -d -L1 /

/
├── bin -> usr/bin
├── boot
├── dev
├── etc
├── home
├── lib -> usr/lib
├── lib64 -> usr/lib
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin -> usr/bin
├── srv
├── sys
├── tmp
├── usr
└── var

18 directories
```

* bin or /usr/bin or /sbin are symlinked as you can see in the tree output above. They are for binary programs. 

* /boot is where the bootloader stores files needed in the boot process such as initramfs, conf files and more.

* /dev is for devices and since everthing in Linux is a file here are hardware represented as files

* /etc is for host-specific system-configuration files like fstab(mounting of partitions)

* /home is where the users of the system lives and stores their files. A machine user does not need a home and can be created whitout one.

* /lib is for shared libraries and kernel modules

* /lib64 is for 64bit share libraries, in modern Linux all libs are found in /usr/lib

* /mnt is for manual mounting point

* /opt add-on application software

* /proc de-facto standard Linux method for handling process and system information

* /root home folder for the root user.

* /run runtime variable data

* /sbin same as /usr/bin

* /sys information about devices, drivers, and some kernel features is exposed. Linux only

* /tmp for temporary files will be wiped on reboot

* /usr stands for UNIX/User System Resources and contains shareable,read-only data.

* /var variable data files. includes spool and administartive and logging data also transient and temporary files


### Installation 
in this case enterprise linux, [AlmaLinux 8](https://almalinux.org/) which is a bug by bug reproduction of the Red Hat Enterprise Linux.
DD the iso to an usb stivk and boot, follow the graphical instructions. 

### Remote installation

### The boot process
### Server from GUI and CLI
### Updating and maintinace
### Standars input/output and error
### Runtimes ??
### Basic commands
### Linking
### Nano/Vim the text editors
### tar and stuff
### man, info and helpers 
### Grep and regular expressions
### yum/dnf packages repo config
### ssh server and client key-based auht
### ntp time sync
### scp copying files over network
### listing and managing Linux processes
### file permissions
### partitioning disks
### Lvm create,extend reduce
### swap 
### creating users and groups
### modify user , password age
### deleting users snd groups
### files and directory permissions
### ACL 
### GID, UID and sticky bit
### Sudo
### Networking static ip
### firewalld 
### SELinux
### Crontab
### RPM/YUM installing and updating
### Containers
### inspect container images
### Container management
### more containers , this should be one topic
### VNC install and configure
### NFS install and configure server/client
### SMB samba




### Improving Command-line productivity


We start the course by learning how to be more effective with the BASH shell.
A simple bash script.


### Sources 
* [Tech Arkit Youtube](https://www.youtube.com/watch?v=-wNfs5fRazI)
* [MyLinuxGig Youtube](https://www.youtube.com/watch?v=3Qo5_Is0VsY)
* [Udemy course by Imran Afzal](https://www.udemy.com/course/unofficial-linux-redhat-certified-system-administrator-rhcsa-8/)
