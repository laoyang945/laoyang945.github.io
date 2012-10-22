---
layout: post
title: '人人网(校内网)日志导出方法'
date: 2010-2-19
wordpress-id: renren-blog-export
comments: true
---
<span style="color: #ff0000;"><strong>[2010年3月31日更新]</strong></span>

新增功能：导出为article.xml，直接可以在wordpress里面通过RSS导入，其他博客服务未测试。

<a href="http://www.uushare.com/user/laoyang945/file/2806841" target="_blank">点击这里</a> 下载脚本文件，用命令行运行xiaoneibackup20100331.py即可

<strong><span style="color: #ff0000;">[2010年2月19日更新]</span></strong>

感谢<a href="mailto:ht.simple.happy@163.com">elfin</a>的工作，使得原来的人人日志导出脚本能够继续使用下去。他在邮件中提到：“今天用工具分析了下renren的http，发现主要原因是Content-Encoding使用了gzip。直接用python的解码模块解码即可。”解决了原来我说的乱码问题。

<span style="color: #ff0000;"><strong>使用方法：</strong></span>
<ol>
	<li>下载python2.4或者2.6版本。（因为python.org/download被不可思议的墙掉了，所以不给链接，请自行搜索下载）</li>
	<li>下载脚本</li>
	<li>在命令行（开始-运行-cmd）中执行脚本</li>
	<li>输入邮箱和密码，脚本就会自动下载你的日志到同目录下的article.xml</li>
</ol>
已知问题：
<ol>
	<li><span style="text-decoration: line-through;">人人网的日志计数可能有误，因此实际下载日志数会小于等于显示日志数</span></li>
	<li>不能下载图片，不能下载评论</li>
	<li><span style="text-decoration: line-through;">导出的文件不能直接导入wordpress。</span></li>
</ol>
