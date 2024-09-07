---
layout: post
title: Github pages 如何使用cloudflare 搭建个人博客
categories: Blog
description: Github pages 如何使用cloudflare 搭建个人博客 
keywords: netgear, R6300，mysql5
---
1、将域名托管到Cloudflare
进入Cloudflare官网注册账号后，点击右上角的add site添加站点。输入要托管的域名，套餐选择free免费版，点击继续。
![](/cloudflare-domain-name.png)

2、点击自定义域名 设置域名
![](/cloudflare-domain-name-1.png)

3、点击 workers-and-pages
构建指令： JEKYLL_GITHUB_TOKEN=xxxxx bundle exec jekyll build
注意：xxxxx需要替换成自己的github token
构建输出目录：/_site
根目录：/


