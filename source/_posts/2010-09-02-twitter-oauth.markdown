---
layout: post
title: '9月1号之后Twitter访问方法汇总[随时更新]'
date: 2010-9-2
wordpress-id: twitter-oauth
comments: true
---
9月1号之后，twitter关闭了basic auth的连接方式，只允许直连或者OAuth，原来的客户端不能用了怎么办？下面总结了一下这两天在推特上看到的解决方案（如果有失效的麻烦留言指出）
<ul>
	<li>首先当然是直接翻墙 （VPN/SSH，推荐用SSH，实在不行GAE也可）</li>
	<li>搭一个<a href="http://code.google.com/p/rabring/" target="_blank">Rabring</a>，或搭建一个支持OAuth的API（教程有这几篇：<a href="http://hiapk.com/thread-316013-1-1.html" target="_blank">搭建支持OAuth验证的twitter api </a>，<a href="http://timewilltell.me/2010/07/update-gae-oauth-api-simple-way-point.html" target="_blank">GAE OAuth API简单点的方法</a>，<a href="http://timewilltell.me/2010/05/gaes-api-methods-built-oauth.html" target="_blank">GAE建oauth的API方法</a>，<a href="http://bbs.dospy.com/thread-7448213-1-190-1.html" target="_blank">速度就是一切！Gae上快速搭建支持oauth的API简易教程</a>，<a href="http://blog.newchen.com/post/1389" target="_blank">用GAE搭建自己的个性化推҉特҉API</a>，<a href="http://www.iteeyan.com/2010/09/netputweets-oauth-login/">不用翻墙，OAuth登录奶瓶腿客户端的方法</a>，<a href="http://7lemon.info/2010/05/oauth-twip.html">轻松搭建oauth twip(PHP)</a>+<a href="http://blog.csdn.net/Raptor/archive/2010/09/03/5861770.aspx" target="_blank">带OAuth的twip安装手记</a>，<a title="Permanent Link to 在alwaysdata免费空间上架设twip oauth api 4" rel="bookmark" href="http://denqjinq.appspot.com/2010/09/twip_oauth_api_alwaysdata">在alwaysdata免费空间上架设twip oauth api 4</a>）或者用<a href="http://www.cn4iran.org/itap/" target="_blank">这个API</a></li>
	<li><a href="http://wowubuntu.com/oauth-twitter.html" target="_blank">Linux下几个支持OAuth的客户端</a></li>
	<li>嫌麻烦的话试试发送一封邮件到mytwitterclient@gmail.com 或者以“红杏”为题发送邮件到jayznbjay@gmail.com</li>
	<li>手机上推，找不到API就用snaptu好了(手机浏览器访问m.snaptu.com)</li>
	<li>手机访问dabr.in，或者http://rabr.fishnote.net/login.php，http://t.caodan.net/enter.php，http://caoni.ma，http://izhe.tk/t/login.php，http://t.wcht.net/login.php https://t.orzdream.com  https://tuite.im</li>
	<li>建一个mixero可用支持OAuth的API比较麻烦，请自行搜索解决方案。</li>
</ul>
总之在这个国家，你必须时时刻刻学习先进的科学技术，真是催人奋进。

摘录三条推文：
<blockquote>@iamzzm: 作为一个纯正文科生，我鄙视一切自以为是文科生就可以不懂得翻墙不寻求解决不求进取的人们

@xiange: Twitter API 改成 OAuth 了，立马很多人就上不来了，这就是只满足发推底线，不向翻墙高标准看齐的坏处。闹饥荒的年头，家里床底下不藏几缸米就不算会过日子。

@nososo: 听说今天能上推的都是可fo之人,于是果断求fo</blockquote>
