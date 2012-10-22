---
layout: post
title: '用Vimperator配合Zotero实现一键收集'
date: 2010-5-15
wordpress-id: vimperator-zotero
comments: true
categories: [Vimperator, Zotero]
---
其实，Zotero默认的摘录功能不是那么强大，而且必须在激活zotero面板的情况下才能用快捷键新增便签，抓取网页快照等，操作上不是那么方便。前几天在Zotero的论坛上瞎逛的时候，发现一个哥们用Vimperator这个扩展配合Zotero可以用快捷键抓取文献信息，<strong><span style="color: #ff0000;">我研究了下，发现不仅可以一键抓取文献信息，还可以一键呼出便签窗口，一键抓取选中文字和一键抓取网页。</span></strong>


使用Vimperator之前，希望你对它有一定的了解，可以在搜索一下相关教程然后再进行安装，否则重启Firefox之后可能会不知道怎么办。

下图就是我的Firefox安装Vimperator之后的效果图，使用Opera的主题，非常简洁。Vimperator让我少装好几个插件，比如personal menu, keyconfig, is.gd, paste and go等。如果你想保持Firefox原本的菜单栏，工具栏和书签栏，在配置文件里面加上 `set gui=all`即可。

<img src="http://static.flickr.com/4009/4607962094_c5baca092f.jpg" border="0" width="500" />

在使用快捷键收集之前，需要先激活Zotero面板一次，默认快捷键是Ctrl+Alt+z，之后就可以关闭Zotero面板。

Vimperator命令行中，抓取页面的命令是`js ZoteroPane.addItemFromPage();`，可以在配置文件中做一个快捷键映射实现一键抓取。

<img src="http://static.flickr.com/3411/4607963416_fec41b2520.jpg" border="0" width="500" />

抓取文献信息的命令是`js Zotero_Browser.scrapeThisPage();`

打开便签窗口的命令是`js ZoteroPane.openNoteWindow();`

<img src="http://static.flickr.com/1063/4607962552_40b4b03cf5.jpg" border="0" width="500" />

把选中内容抓取为便签的命令是`js ZoteroPane.newNote(false,false,getBrowserSelection(),gLastValidURLStr);`

<img src="http://static.flickr.com/1418/4607963794_97f5e5772b.jpg" border="0" width="500" />

在Vimperator的帮助下，你的Zotero收集便捷度已经超过了其他任何的收集工具，还有什么能比一键收集还快呢？
