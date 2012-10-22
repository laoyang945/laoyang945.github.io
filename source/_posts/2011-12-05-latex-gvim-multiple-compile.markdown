---
layout: post
title: 'LaTeX+gVim多次编译设置'
date: 2011-12-5
wordpress-id: latex-gvim-multiple-compile
comments: true
categories: [Vim, LaTeX]
---
如果你是按照我前一篇文章设置的话，文章中有参考文献或者目录而需要多次反复编译的时候，可能会出问题，需要的东西没有显示出来。

解决方案是，修改Vim安装目录\vimfiles\ftplugin\latex-suite\texrc，将
	TexLet g:Tex_MultipleCompileFormats = 'dvi'
修改为
	TexLet g:Tex_MultipleCompileFormats = 'pdf,dvi'
即可对pdf格式的输出进行多次编译
