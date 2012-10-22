---
layout: post
title: '设置本地文件夹为盘符'
date: 2008-11-24
wordpress-id: mapping-folder-to-disk
comments: true
---
<p>&#160;&#160;&#160; 今天下载课件的时候，觉得自己放置课件的目录E:\My Files\00_School About\2008_Fall\还是不太好找的，特别是如果之前下载文件的保存路径在其他地方的话，还要点好几次才能定位到这里。于是我想把这个文件夹直接设置为一个盘符。</p>  <p>&#160;&#160;&#160; Google之后，很顺利的完成了，利用ms-dos自带的subst命令就可以做到。步骤是这样的：</p>  <ol>   <li>开始-运行-输入cmd回车 </li>    <li>在命令行窗口中输入subst [待分配的盘符号：]空格[映射的文件夹路径]，回车即可</li> </ol>  <p>&#160;&#160;&#160; 我的命令是subst z: “e:\my files\00_school about\2008_fall”。因为在命令行之下路径是不能包含中文和空格的，所以要用引号引起来。下图是用了这个命令之后的硬盘，是不是多了一个？</p>  <p>&#160;&#160;&#160; <a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20080921-173417.png"><img title="2008-09-21_173417" style="border-top-width: 0px; display: inline; border-left-width: 0px; border-bottom-width: 0px; border-right-width: 0px" height="117" alt="2008-09-21_173417" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2008/11/20080921-173417-thumb.png" width="116" border="0" /></a> </p>  <p>&#160;&#160;&#160; 但是，这个命令的有效期只到关机，下一次再开机的话这个映射的盘符就不存在了。要解决这个问题，我猜有两个办法：1）不关机，只是休眠或者待机；2）将subst命令加入c盘下面的autoexec.bat文件中，以后开机就能自动执行一遍了。</p>  <p>&#160;&#160;&#160; 把本地文件夹映射为盘符，在临时频繁需要的文件夹操作上很有好处。</p>
