---
layout: post
title: "获取Picasa相册中所有图片真实地址的脚本"
date: 2012-02-19 10:31
comments: true
categories: [blog]
---

用了新的域名，新的博客架构，还是在发愁图床用哪个。图床和博客分开主要是为了以后万一搬家比较方便。看了一圈发觉还是picasa不错，我本来就是Gmail的付费扩容用户，容量就有20G，而且picasa可以用https访问，在Google Reader或者Gmail里面查看图片也不会报错。

但是picasa就是获取真实图片地址比较麻烦，不管是手动右键还是在右边的link里面做选择。于是自己尝试写了一个python脚本，用于获取公开相册下的各图片地址

使用方法，双击运行输入相册地址（最好是https，因为http的ggpht.com被墙），然后在脚本路径下就会有一个url.txt文件，里面每一行就是一幅图片的地址了。

{% include_code picasa.py %}
