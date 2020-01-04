---
title: hexo 安装
categories:
  - 技术
tags:
  - hexo
  - 安装
date: 2020-01-04 14:35:52
---

官方网站：
https://hexo.io/

开发环境搭建：
``` bash
$ npm install hexo-cli -g #安装脚手架
$ hexo init blog #初始化项目
$ cd blog #进入项目目录
$ npm install #安装依赖
$ npm install hexo-deployer-git –save #安装发布插件
$ npm install hexo-git-backup --save #hexo backup or hexo b 备份hexo
```

方便前准备：

在本机生成public key
``` bash
$ ssh-keygen -t rsa -b 4096 -C "xxx@xxx.com"
```
然后在`#user_id/.ssh`目录下会生成两个文件，id_rsa.pub和id_rsa.
然后登陆github，在SSH设置页面添加上刚才的public key文件也就是id_rsa.pub的内容即可。

发布：
``` bash
$ hexo clean #清理
$ hexo generate #生成
$ hexo deploy #上传
```

开发环境提供了实时预览的方式，不需要每次都generate，执行命令：
``` bash
$ hexo generate -w
```

常用命令与简写命令：
``` bash
$ hexo n == hexo new
$ hexo generate(hexo g) #生成静态文件，会在当前目录下生成一个新的叫做public的文件夹
$ hexo new "postTitle" #新建博客文章
$ hexo new page "pageTitle" #新建1个页面
$ hexo server(hexo s) #启动本地web服务预览(加参数--debug,用于调试，如：hexo s --debug)
$ hexo deploy(hexo d) #部署播客到远端（比如Github,coding,heroku等平台）
```
