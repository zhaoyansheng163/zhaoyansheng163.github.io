---
layout: page
title: 关于
description: 关于
keywords: 赵延生
comments: true
menu: 关于
permalink: /about/
---

我是赵延生。

一个IT爱好者和工作者，欢迎一起学习交流。

Apache Eventmesh Contributor

参与的开源项目：

Apache Eventmesh： https://github.com/apache/eventmesh/

gitlab到gitea迁移工具： https://github.com/h44z/gitlab_to_gitea

IOS作品：
私家藏书： https://apps.apple.com/cn/app/%E4%B9%A6%E8%99%AB-%E5%9B%BE%E4%B9%A6%E6%95%B4%E7%90%86/id6670142604

曾创办网站：AppInventer论坛  www.appinventor.com.cn  
《人人都能开发安卓App：App Inventor 2应用开发实战》  书籍是我这个网站三位资深版主所写，其中一位是律师朋友。
![](/images/posts/Blog/about-anninventor.png)

感谢支持正版书籍：https://e.jd.com/30189868.html

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## 技能关键词

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
