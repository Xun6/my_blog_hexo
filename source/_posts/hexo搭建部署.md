---
title: hexo搭建部署
date: 2022-08-31 11:19:47
tags:
- hexo部署
comments:

---


## 1、搭建安装 hexo
请参考官方文档：https://hexo.io/zh-cn/docs/setup

## 2、将 Hexo 部署到 GitHub Pages
- 安装 hexo-deployer-git

	`npm install hexo-deployer-git --save`

- 在github上新建一个新的仓库，例如 *Myblog.github.io*

- 修改 Hexo配置文件`_config.yml`,将 url 修改为 `https://<你的 GitHub 用户名>.github.io/<repository 的名字>`、将 root 的值修改为 `/<repository 的名字>/`
{% asset_img QQ截图20220831105133.jpg 'url配置修改' %}


- 添加`_config.yml`配置
![](QQ截图202.jpg)

- 运行` hexo clean` && `hexo deploy` （注意：每次本地修改编辑后，再执行，部署到GitHub上）

- hexo s 开启服务，查看站点是否部署成功