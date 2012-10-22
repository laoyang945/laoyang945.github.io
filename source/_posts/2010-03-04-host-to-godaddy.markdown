---
layout: post
title: '主机转移到Godaddy'
date: 2010-3-4
wordpress-id: host-to-godaddy
comments: true
---
最近有挺多想法的但是一直都没写，原因就是博客要更换主机

自从开设独立博客以来就用的是dreamhost的主机，用了有小半年了吧，有几个问题搞得我有点不爽
<ul>
	<li>慢</li>
	<li>时不时就断掉连不上，没有任何解释……</li>
	<li>这个主机我还拿来用MyEnTunnel，所以……你懂的</li>
</ul>
那天在twitter上找<a href="http://twitter.com/iamzzm">@iamzzm</a>合租了这个Godaddy的空间，经过一番折腾，终于把整个主机转移过来了。其中有几个地方需要注意的：
<ol>
	<li>Godaddy的域名只能绑定1个Godadday的主机，原来我绑定过买域名的时候送的那个免费空间，所以@iamzzm一直不能帮我绑定。后来发现了这个问题，解除那个免费空间的绑定就好。（Godaddy的解除绑定的提示做得像广告一样，让我一直在等弹出的对话框……）</li>
	<li>用<a href="http://www.backupify.com/" target="_blank">Backupify</a>这个网站的服务很不错，定期能帮你备份文件和数据库。这次搬家我就是直接把Backupify备份的文件上传到FTP，数据库文件导入到新的数据库（不过好像少了几天的评论？）。导入之后记得修改wp-config.php里面数据库相关的url还有用户名密码</li>
	<li>Backupify导出的数据库文件导入到新数据库的时候，访问wordpress有乱码，需要在wp-config.php里面加一行define('DB_CHARSET', 'utf8');因此前几天有人访问我的博客的时候全是？？？，居然还留言了（好像是<a href="http://www.xyzlove.com" target="_blank">午夜兰花</a>？怎么网站无法访问了？），当然留言也是乱码，我看不见。</li>
</ol>
在搬家的时候还帮<a href="http://twitter.com/bigzui">@bigzui</a> 建了一个独立的博客，域名是<a href="http://bigzui.info" target="_blank">bigzui.info</a>，哈哈，大家可以去看看，一个很有趣的大一学生。
