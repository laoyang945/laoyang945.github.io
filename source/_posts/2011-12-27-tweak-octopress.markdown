---
layout: post
title: "Octopress修改样式及加速预览"
date: 2011-12-27 10:03
comments: true
categories: [blog, Octopress]
---
样式主要是要修改/sass/custom/\_style.scss这个文件，比如现在我的文章标题就是
	.entry-title{font-size: 1.5em;}
这个文件最后读入，覆盖之前的设置，生成对应的screen.css文件

另外，如果需要编写编改，而文章太多造成编译缓慢的话，可以用rake isolate这个命令。比如当前这一篇可以用
	rake isolate[tweak-octopress]
编译，这个时候ruby会把之前编译好的都到source/\_stash，只编译这一篇。这样用preview看比较快。要发布的时候再用
	rake integrate
	rake generate
	rake deploy
就好
