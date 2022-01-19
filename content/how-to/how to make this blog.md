+++
title = "Making this blog"
weight = 1

[taxonomies]
tags = ["zola", "git", "cloudflare", "cloud"]
+++

# Intro

This is a short walktrough of how this blog was made.
What is a ststic site generator
What is the spec I am looking for

# Choosing static site generator

There is a jungle out there, waht should you choose ?
This time I went with feel rather than some metric. I tried a couple of the most popular ones and when I got to Zola ??I just went with that.
This is a list of [Static site generators](https://jamstack.org/generators/)
Hugo is a well known and a good alternative.
makesite.py is interressting, since I know some python but it looks like the project is not very active . [Nikola]https://getnikola.com/ is another Python alternative. but for now we will stay with Zola.  
Zola is fast and intergates very well with the hosting solution I choose to go with. It is written in Rust and is easy to install and work with . It uses the [Tera template format](https://github.com/Keats/tera). The workflow is similar to the other static site generators in that it revolves around editing templates and writing markdown.

# Installing Zola

On Arch Linux:

```Bash
pacman -S zola
```
From their documentation [install Zola](https://www.getzola.org/documentation/getting-started/installation/)


# Configuring Zola

# Hosting

# Conclusion