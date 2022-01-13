+++
title = "I like Linux and open source"
date = 2019-02-02
weight = 2

[taxonomies]
tags = ["linux", "hello"]
+++

The intent is to blog, mostly how to style and maybe some rants about technology generally and Linux, open source and Ops specifically. 
I am studying K8S and GitOps a the moment. 

Linux is the best, I run Arch btw. I also run NixOS and Talos on metal. In a container nobody cares.


[linux.com](https://www.linux.com/)

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:1.14.2
        ports:
        - containerPort: 80

```

<!-- more -->




