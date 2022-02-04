+++
title = "Hello World!"
date = 2021-12-12
updated = 2022-01-15
description = "First post :-)"

[taxonomies]
tags = ["hello"]
+++

Hello World! This is the first post. Just testing some markdown tags.

<!-- more -->

[linux.com](https://www.linux.com/)

```rs
let highlight = true;
```

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





