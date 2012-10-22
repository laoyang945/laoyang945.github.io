---
layout: post
title: "Vimperator配合Evernote进行一键悦读及收集"
date: 2012-05-31 14:17
comments: true
categories: [Vimperator, Evernote]
---
Vimperator是一个极其好用的Firefox扩展，让你对浏览器的操作完全的Vim化，所有的按键都用上。我原来也写过好几篇介绍它的文章。

今天要介绍的就是在Vimperator下如何一键能够把当前网页用Evernote的Clearly（悦读）进行重新排版，以及如何一键把浏览器中的各种内容发送到Evernote。首先你得安装对应的Firefox扩展，地址在[这里](https://addons.mozilla.org/en-US/firefox/addon/clearly/)和[这里](https://addons.mozilla.org/en-US/firefox/addon/evernote-web-clipper/)

首先，只用Clearly转换的命令是
	:js __readable_by_evernote.readable_by_evernote__menu__call(buffer.URL)

用Clearly转换并存储到Evernote的命令是
	:js __readable_by_evernote.__readable_by_evernote__launch(true)

把选中内容发送到Evernote的命令有好几个：
	evernote_doAction( document.popupNode, 'CLIP_ACTION_FULL_PAGE' );
	evernote_doAction( document.popupNode, 'CLIP_ACTION_IMAGE' );
	evernote_doAction( document.popupNode, 'CLIP_ACTION_SELECTION' );
	evernote_doAction( document.popupNode, 'CLIP_ACTION_URL' );
	evernote_doAction( document.popupNode, 'NEW_NOTE_ACTION' );
大家分别试试就知道每一个的用处，但我觉得第三个clip\_action\_selection应该是最常用的吧。

我还录了一小段视频，可以看看使用的效果，地址在[这里](http://www.youtube.com/watch?v=rknrtX2gL0Q)

[参考](http://d.hatena.ne.jp/cd01/20120505/1336201859)
