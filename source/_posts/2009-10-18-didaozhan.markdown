---
layout: post
title: '地道战的打法'
date: 2009-10-18
wordpress-id: didaozhan
comments: true
---
<p>假设你现在已经挖好了一个地道，从下面绕过了墙。你用这个地道逛得很爽的时候，突然发现地道是有人流量限制的，那怎么样才能让你的某些指定流量从这个地道中走呢？（如果读不懂这段，后面也没必要看了）</p>  <p>假设你的地道是socks5的，地址是127.0.0.1:1234</p>  <p><strong>1.firefox+autoproxy插件</strong></p>  <p>这没什么好说的，autoproxy的地址在<a href="http://www.autoproxy.org/">http://www.autoproxy.org/</a>，配置代理就可以</p>  <p><strong>2.其他浏览器，可以使用privoxy+pac自动配置脚本</strong></p>  <p>先在privoxy的配置文件最后加入一行</p>  <p>forward-socks5 / 127.0.0.1:1234 <font color="#ff0000">.</font></p>  <p>这样就把所有对privoxy提供的HTTP代理（默认8118端口）的访问（/）转到你socks5的代理上了，<font color="#ff0000">不要忘记最后的那个点</font></p>  <p>然后打开一个文本文件，然后像下面这样写一段，假设保存为d:\didaozhan.pac文件（直接修改后缀即可）</p>  <blockquote>   <p>function FindProxyForURL(url, host) { </p>    <p>if (shExpMatch(url, “www.google.com/search?*”)) { return “PROXY 127.0.0.1:8118″; } </p>    <p>if (shExpMatch(host, “*163.com”)) { return “PROXY 127.0.0.1:8118″; } </p>    <p>return “DIRECT”; </p>    <p>}</p> </blockquote>  <p>不管学过还是没学过编程的都能看懂吧，这个函数有两个参数，一个是地址，一个是主机名称。第一个if判断如果是google搜索的url，用代理，另一个if判断如果是163站内的东西，那一律用代理。如果这两条都不满足的话，直接连过去就好。你可以无限扩充这个if列表。同时因为是用正则表达式处理的，形式上还可以更灵活。</p>  <p>在浏览器中设置自动配置脚本地址为<a href="file://d:/didaozhan.pac">file://d:/didaozhan.pac</a>，<font color="#ff0000">注意file后面是两个斜杠，然后路径的写法也稍有不同。</font></p>  <p><strong>3.照理来说只用privoxy也是可以的，就是forward那里要针对不同的网站做修改，但是我没成功过。如果知道怎么弄的请留言说明。</strong></p>
