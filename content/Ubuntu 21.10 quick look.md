+++
title = "Quick look at Ubuntu 21.10"
date = 2022-02-01
updated = 2022-02-05
description = ""
[taxonomies]
tags = ["how-to", "Linux", "Ubuntu", "beginner", "quick look", "GNOME"]
+++

# Let's take a look at Ubuntu 21.10

Ubuntu is one of the most popular Linux distributions. The first release was 04.10 back in 2004. It started as a project to make debian more user friendly. They follow a six month release schedule with a long-term support release every two years. The current long-term release is the 20.04 version.
Under Canonicals stewardship it has grown to be almost synonomous with Linux espescially on the desktop. 
Although there always were good alternatives, and recently there has been some serious contenders like Pop_OS, Solus and Manjaro Linux. Even the classic distors like Fedora and Open Suse have been putting out some stellar releases.



<!-- more -->

# Downloading the isos

The first thing we need is the OS, Ubuntu provides iso images of their OS freely from their website. 
Head over to the Download page: [Ubuntu Download](https://ubuntu.com/download/desktop)

# Making a bootable usb
First descision to be made, install to metal or virtual machine.
If you want to install to your physical machine, first you have to burn your iso to an usb-key.
Here are three options which should cover most use cases, but there are more ways to do this. If you are so inclined, it should not be very difficult to find using [DuckDuckGo](https://duckduckgo.com/) or any similar search engine.

#### Etcher
One of the most popular is etcher, it is an electoron app and is availiable on the major proprietary platforms. 

* [Etcher download](https://www.balena.io/etcher/)

Etcher is very easy, just pick the isop, chose the drive and hits the "Flash!" button.

<img src="/img/ubuntu2110/etcher.png" width="600" class="center">

#### GNOME-Disks
But if you alredy are on GNOME you could use gnome disk, like this:

Choose the restore image option.
<img src="/img/ubuntu2110/disk-1.png" width="600" alt="Hello" class="center">

Pick the iso you want to use and hit start restoring.
<img src="/img/ubuntu2110/disk-2.png" width="600" class="center">

#### DD

Or you could use the trusty old dd utility from the command line.

```sh

cd to/the/folder/of/your/iso/

sudo dd if=ubuntu-21.10-desktop-amd64.iso of=/path/to/usb-stick bs=1M && sync

```

#### Install using virt-manager 

Ubuntu boots you straight into a live session, where you can choose whether you want to try out the desktop or if you want to install the OS to disk. If you are unsure whether all your hardware is supported, the live-session is a good opportunity to test and see what works and what doesn't.
Highly recomended if you want to install to a laptop from a non-linux vendor.

<img src="/img/ubuntu2110/ubuntu-1.png" width="600" class="center">




# Conclusion
