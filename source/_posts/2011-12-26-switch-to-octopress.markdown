---
layout: post
title: "博客迁移到Octopress"
date: 2011-12-26 14:45
comments: true
categories: blog
---
我的博客现在迁移到了Octopress，一个基于静态页面的博客系统。这样做的好处有：

- 访问速度快
- 可以放在github/aws上，免得自己再找主机，还可以绑定域名（不过我的blog域名被封了，暂时就用github提供的吧）
- 数据导入导出简单
- markdown语法，用vim写起来方便
- 配置容易

rss的地址不变，依然是<http://feeds.feedburner.com/laoyang945>

简要介绍一下Windows下如何使用github+Octopress

- 下载[Git](http://git-scm.com/),[RubyInstaller](http://rubyinstaller.org/), [Development Kit](http://rubyinstaller.org/downloads/)，并分别安装。安装git的时候记得让它写入path
- 环境变量设置HOME=你放证书的路径，LC\_ALL=zh\_CN.UTF-8, LANG=zh\_CN.UTF-8
- 按照github的说明设置git
- 以后的步骤可以参考[octopress官网](http://www.octopress.org)
