---
layout: post
title: '人人网日志导出脚本更新(2011-05-23)'
date: 2011-5-23
wordpress-id: renren-article-export-update
comments: true
---
因为人人老改url啊，ajax异步访问什么的，原来的导出脚本失效

昨天更新了一下

下载地址在<a href="http://u.115.com/file/clw5yttf" target="_blank"> http://u.115.com/file/clw5yttf</a>

使用方法

1.首先下载python2.7（2.6也可以）

2.双击运行脚本

3.输入相关信息，那个日志地址需要输入的是最后两组数字，比如你的最新一篇日志地址是http://blog.renren.com/blog/1234567890/1234567890?fromfriendblog，那就输入1234567890/1234567890

4.导出来的文件是wordpress的xml格式，如果需要其他格式的请自行修改代码

运行截图：

<img class="picasa" src="https://lh3.googleusercontent.com/_W7vzKfSkTVE/Tdn4f3F6O9I/AAAAAAAAFsY/rQpZUNfNYYA/s400/2011-05-23%2013%2055%2030.png" alt="" />

还需完善的：导出图片功能，但是这得需要将日志中的图片链接也改为本地的，有点麻烦，有高人愿意接手么？
