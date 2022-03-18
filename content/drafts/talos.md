+++
title = "Talos and metallb"
date = 2021-12-31
updated = 2022-02-01
description = "Creating a cluster"
[taxonomies]
tags = ["k8s", "linux", "talos", "kubernetes", "metallb"]
+++

[Talos.dev](https://talos.dev)
[Metallb](https://metallb.com)

In this post we will install talos on metal with metallb as our loadbalancer.

TAlos is a kubernetes ditribution which focuses on minimizing the OS on which the cluster rums.
For a Linux enthusiast like me it is slightly ironic that one of the selling poits of talos is as lilttle Linux as possible. That means no ssh and no userland at all. With talos you have to embrace an api driven configuration approach. The low base os and the api driven results in a very small attack surface and talos is considered on of the most secure k8s distros. The fact that it is also dead easy to install and maintain is of course a big pluss.

Metallb is an kubernetes loadbalancer service, it provides and easy and straight forward method of exsposing you cluster to the outside world, in my case that means it locally routable inside my nat network. 

