+++
title = "Taking a look at Fedora 35"
date = 2021-12-31
updated = 2022-02-01
description = "Let's check out Fedora 35"

[taxonomies]
tags = ["how-to", "Linux", "Fedora", "beginner", "GNOME"]
+++

Let's take a look at [Fedora Workstation 35](https://getfedora.org/). 

<!-- more -->

Fedora is the upsteam distribution for Red Hat Enterprise Linux and as such is often released with the latest versions of many Linux projects, like GNOME and in this version the new sound subsystem PipeWire.

It currently comes in five different editions.Fedora 35 was released on november 2 2021.
The one we are taking a look at here is the workstation edition which is
the traditional desktop edition. They also offer the Fedora Silverblue edition, which is an imutable desktop where software is installed with flatpak. This is an intersting concept that might be worthy of another post.

It comes with the GNOME desktop, and in the 35 release that would be GNOME 41 which is the latest GNOME release.


[Fedora workstation download direct link](https://download.fedoraproject.org/pub/fedora/linux/releases/35/Workstation/x86_64/iso/Fedora-Workstation-Live-x86_64-35-1.2.iso)

# Installing with Qemu/kvm and virt-manager

 Rule of thumb for me when I try new distors in a vm is to pick 1Gib per cpu core and when trying a deskop I generally stick to 4 cpus and 4Gib of ram. This is reasonable for a desktop install.

After going through the New VM wizard from virt-manager. You should now be booted into a live enviroment like this: 


<img src="/img/install fedora/1-step.png" width="800">

