---
layout: post
title: '如何从校内网导出日志'
date: 2009-7-1
wordpress-id: export-blogs-from-xiaonei
comments: true
---
<p><a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/07/images.jpg"><img title="images" style="border-right: 0px; border-top: 0px; display: inline; border-left: 0px; border-bottom: 0px" height="83" alt="images" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/07/images-thumb.jpg" width="131" border="0" /></a> </p>  <p>校内网的日志功能实在是很糟糕，不能RSS输出，编辑器也很弱，整体架构不开放，万一哪天被杀档了那辛辛苦苦写的日志不就全没了。（还有其他缺点欢迎指出）</p>  <p>所以决定把校内的日志备份出来，以后专心在yo2和葡挞写。</p>  <p>备份方法：</p>  <ol>   <li>在Python的官方网站<a href="http://www.python.org/">http://www.python.org/</a>，下载2.6.2或者2.4.4的python，安装</li>    <li>在<a href="http://cid-fa722330f2b9195d.skydrive.live.com/self.aspx/.Public/xiaonei%7C_backup.py" target="_blank">这里</a>下载网友flydreamersu编写的代码xiaonei_backup.py，原文地址<a href="http://flydreamersu.blogbus.com/logs/38775632.html">http://flydreamersu.blogbus.com/logs/38775632.html</a></li>    <li>开始-运行-cmd，然后cd到你保存xiaonei_backup.py的目录下</li>    <li>输入xiaonei_backup.py 用户名 密码，回车</li>    <li>耐心等待</li>    <li>最后导出的日志在同目录下的blog.txt文件，当然你可以改成html或者xml</li> </ol>  <p>这个脚本还是有一点不足的，第一是最后总提示错误，后来发现是下标越界了；第二就是图片不能保存下来，我有空研究下python看看能不能把图片一起保存了。</p>
