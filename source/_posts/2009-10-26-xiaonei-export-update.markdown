---
layout: post
title: '校内网/人人网 日志导出脚本更新'
date: 2009-10-26
wordpress-id: xiaonei-export-update
comments: true
---
<strong><span style="color: #ff0000;">[2010-01-29</span><span style="color: #ff0000;">]</span></strong>

原有脚本已经无法读取人人网的任何内容，怀疑服务器端做了加密，载下来的html都是乱码。且就在1-17脚本更新之后几天人人修改了日志的链接格式。

本人精力和能力有限，停止更新此脚本，希望其他高手能接手。

下载地址点<a href="http://cid-6fcda80e41592c52.skydrive.live.com/self.aspx/Public/xiaonei%5E_backup20100117.py" target="_blank">这里</a><strong><span style="color: #ff0000;">[2010-01-17更新]</span></strong>

2010-01-17更新如下：
<ol>
	<li>解决因为校内日志链接格式变更而造成的错误</li>
	<li>登录HTTP报头修改</li>
</ol>
2009-10-26更新如下
<ol>
	<li>修改域名和登陆地址</li>
	<li>post数据中增加origURL</li>
	<li>用户名和密码按提示输入</li>
	<li>header中增加一些参数，使得不会发生HTTP 500错误</li>
</ol>
使用方法：安装python后，<span style="text-decoration: line-through;">直接双击运行xiaonei_backup.py即可。在python2.4下使用正常，如果有问题请留言</span>感谢午夜寒刀的提示，最好cmd到脚本所在的目录下，然后运行这个脚本
