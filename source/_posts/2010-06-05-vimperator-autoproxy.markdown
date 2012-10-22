---
layout: post
title: '用Vimperator切换Autoproxy代理方式'
date: 2010-6-5
wordpress-id: vimperator-autoproxy
comments: true
---
如果用Vimperator把状态栏和工具栏都隐藏起来了，如何切换Autoproxy的代理方式（自动/禁用/全局）呢？

命令很简单：

:set! extensions.autoproxy.proxyMode=auto&lt;CR&gt;:echo "auto"&lt;CR&gt;

其中&lt;CR&gt;表示回车，echo "auto"表示在命令栏的位置显示一下“auto”。全局代理只需要把proxyMode=auto改为global即可。

如何找到这些Vimpertor可运行的命令？在set! extensions.之后输入关键字按Tab键试试～
