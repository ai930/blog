---
title: hexo 给自己的博客添加萌宠或萌妹子
categories:
  - 技术
tags:
  - hexo
  - 网站美化
date: 2020-01-04 14:29:28
---

## 1. 获取

```undefined
npm install --save hexo-helper-live2d
```

## 2.选择自己喜欢的萌妹子
可以到github中查看，选择喜欢的妹子造型
```rust
live2d-widget-model-chitose
live2d-widget-model-epsilon2_1
live2d-widget-model-gf
live2d-widget-model-haru/01 (use npm install --save live2d-widget-model-haru)
live2d-widget-model-haru/02 (use npm install --save live2d-widget-model-haru)
live2d-widget-model-haruto
live2d-widget-model-hibiki
live2d-widget-model-hijiki
live2d-widget-model-izumi
live2d-widget-model-koharu
live2d-widget-model-miku
live2d-widget-model-ni-j
live2d-widget-model-nico
live2d-widget-model-nietzsche
live2d-widget-model-nipsilon
live2d-widget-model-nito
live2d-widget-model-shizuku
live2d-widget-model-tororo
live2d-widget-model-tsumiki
live2d-widget-model-unitychan
live2d-widget-model-wanko
live2d-widget-model-z16
```

例如选择： live2d-widget-model-miku

- 安装

```undefined
npm install live2d-widget-model-miku
```

## 3. 配置

在站点的 _config.yml 下配置

```bash
live2d:
  enable: true
  scriptFrom: local
  model:
    use: live2d-widget-model-miku
  display:
    position: right
    width: 150
    height: 300
  mobile:
    show: true
```
