---
layout: post
title: 网件 netgear R6300 如何安装mysql5
categories: Route
description: 网件 netgear R6300 如何安装mysql5
keywords: netgear, R6300，mysql5
---

1、先安装 optware 
参考路由器R6300 SVN的安装

2、安装mysql 
先更新 
ipkg-opt update 

安装依赖的库 
ipkg install ncurses-dev 
ipkg install ncursesw 
ipkg install ncursesw-dev 

安装mysql5 
ipkg-opt install mysql5

如果已经安装mysql4  先卸载，并删除目录 /opt/var/lib/mysql   /opt/lib/mysql

3、启动 
直接使用mysql4的启动方法  
/opt/etc/init.d/S70mysqld start 
会报错，
mysql5需要指定用户的 
/opt/etc/init.d/S70mysqld start --user=root 

参考来自  http://mybookworld.wikidot.com/forum/t-748781
