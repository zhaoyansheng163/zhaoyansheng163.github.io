---
layout: post
title: gitlab迁移到gitea可行方案
categories: Blog
description: gitlab迁移到gitea可行方案
keywords: 
---
gitea与gitlab优势比较明显，实际占用资源占比大约 1:4

gitlab迁移所有仓库到gitea，目前有自动化脚本，但是有个bug需要修复

原始自动化迁移工具

https://github.com/h44z/gitlab_to_gitea

遇到的问题：

import failed: {"message":"Authentication failed: Clone: exit status 128 - remote: HTTP Basic: Access denied\nfatal: Authentication failed

问题分析及修复：

对比请求和 gitea的swagger接口文档，发现文件 migrate.py 缺少一个参数："auth_token": "xxxx"   。加上即可解决

 

正常可用的版本：

https://github.com/zhaoyansheng163/gitlab_to_gitea

 
已向原作者提交修复申请： https://github.com/h44z/gitlab_to_gitea/pull/22

 

gitea swagger

http://192.168.1.3:3000/api/swagger#/repository/repoMigrate

