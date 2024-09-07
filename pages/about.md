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
Apache Eventmesh： https://github.com/apache/eventmesh/pull/3064
gitlab到gitea迁移工具： https://github.com/h44z/gitlab_to_gitea


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
