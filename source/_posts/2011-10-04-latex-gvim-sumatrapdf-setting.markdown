---
layout: post
title: 'LaTeX+gVim+SumatraPDF设置'
date: 2011-10-4
wordpress-id: latex-gvim-sumatrapdf-setting
comments: true
categories: [Vim, LaTeX]
---
【本文仅讨论windows平台下设置】

一句话介绍：
<ul>
	<li>LaTeX：所想即所得的科学论文排版工具，介绍见 <a href="http://zzg34b.w3.c361.com/homepage/TeXintroduction.htm" target="\_blank">http://zzg34b.w3.c361.com/homepage/TeXintroduction.htm</a>，<a href="http://liyanrui.is-programmer.com/2009/9/29/Prologue.11788.html" target="\_blank">这里</a>有一篇很有趣的文章介绍TeX的发展（<a href="http://hi.baidu.com/jiyeqian/blog/item/240a01031555d8fe09fa93ac.html" target="\_blank">备用链接</a>）</li>
	<li>gVim：编辑器中的战斗机，介绍见 <a href="http://xbeta.info/vim-tutorials.htm" target="\_blank">http://xbeta.info/vim-tutorials.htm</a></li>
	<li>Sumatra PDF：轻量又快速的PDF阅读器，介绍见 <a href="http://xbeta.info/sumatra-pdf.htm" target="\_blank">http://xbeta.info/sumatra-pdf.htm</a></li>
<!--more-->
</ul>
安装及下载：
<ul>
	<li>LaTeX我推荐安装texlive，在线安装请点<a href="http://www.tug.org/texlive/acquire-netinstall.html" target="\_blank">这里</a>，下载光盘镜像（2.3G）请看<a href="http://www.tug.org/texlive/acquire-iso.html" target="\_blank">这里</a>，运行install-tl.bat进行安装，安装路径不要有空格</li>
	<li>gVim请到官网 <a href="http://www.vim.org/download.php" target="\_blank">http://www.vim.org/download.php</a>，安装路径不要有空格，假设安装到了c:\vim</li>
	<li>latex-vim插件：<a href="http://vim-latex.svn.sourceforge.net/viewvc/vim-latex/trunk/vimfiles/" target="\_blank">http://vim-latex.svn.sourceforge.net/viewvc/vim-latex/trunk/vimfiles/</a> 点页面底部的“Download GNU tarball”即可</li>
	<li>Sumatra PDF <a href="http://blog.kowalczyk.info/software/sumatrapdf/download-free-pdf-viewer-cn.html" target="\_blank">http://blog.kowalczyk.info/software/sumatrapdf/download-free-pdf-viewer-cn.html</a></li>
	<li>一个小补丁 <a href="http://min.us/mTFMMfLs8" target="\_blank">http://min.us/mTFMMfLs8</a>, 感谢原作者liangzi@bbs.ctex.org</li>
</ul>
配置：
<ul>
	<li>将下载的vim-latex-vimfiles.tar.gz解压到c:\vim\vimfiles</li>
	<li> 将sumatraPDF的安装路径和c:\vim\vim73加入环境变量</li>
	<li>修改c:\vim\\_vimrc文件，添加如下几行：</li>
</ul>
	filetype plugin on

	set shellslash

	set grepprg=grep\ -nH\ $*

	filetype indent on

	let g:tex_flavor='latex'

	let g:Tex_DefaultTargetFormat = 'pdf'

	let g:Tex_ViewRule_pdf = 'SumatraPDF -reuse-instance -inverse-search "gvim -c \":RemoteOpen +\%l \%f\""'

	let g:Tex_CompileRule_pdf = 'xelatex --synctex=-1 -src-specials -interaction=nonstopmode $*'
<ul>
	<li>将补丁解压到c:\vim\vimfiles\ftplugin\latex-suite，覆盖compiler.vim文件</li>
</ul>
OK，大功告成了，至于如何使用LaTeX写论文请待下一篇文章
