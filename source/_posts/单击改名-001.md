---
title: 使用教程{一}
date: 2021-01-20 00:35:00
categories: 
- 静态博客编辑器
- 教程
tags: 
- 静态博客编辑器
- 教程

---
# 简介

## 首先,这是一个github内容编辑器
可以方便的增加,删除,编辑github文件
markdown文件还支持实时预览

## 期次,主要定位是静态博客文章管理


支持Hexo、Hugo、jekyll等主流静态博客
并且根据静态博客特点做了很多优化,使大家专注于写文章,而不是折腾什么博客,内容才是王道

* 自定义文章头模板

> 文章头内容繁杂,尤其是个别主题,自定义字段很多 记不住,提前定义好模板,一键插入
(支持多个模板)

* 自定义标签、文章分类

> 提前设置好,一键插入,不用到处扒拉

* 方便的图床

> 博客图片是个问题,本程序支持图片直接粘贴,自动上传图床（sm.ms）,自动插入代码,Ctrl+V搞定一切
还支持Chevereto系列图床（默认路过图床）,也很方便,可自定义选哪家,当然也可自建,选自己

* 一键发布

> 不用99,不用9块9,只需要点一下【发布】按钮

* 支持提建议

> 这一条厉害了,你觉得写博客哪一步繁琐,提给作者,尽力帮大家再简化

* 最后，他是个网页版

> 不用部署环境,不用敲命令行,有浏览器就行,手机也行

# 快速上手,5分钟毕业

> 如果你只是想建个博客,写写文章,看完这一节就毕业了,其他的一概不用看

避免选择恐惧症,这里只介绍一条路,这条路就是

`github+hexo+netlify`


## 注册github并获取token
[点这里](https://github.com/settings/tokens "点这里"),生成一个token,权限勾选`repo`

## 一键部署到netlify

[![一键部署](https://d33wubrfki0l68.cloudfront.net/65a18ef24e011fbc0b5ddb411d611c0e1d1111a6/17e0b/images/deploy-button.svg "一键部署")](https://app.netlify.com/start/deploy?repository=https://github.com/sbedit/sbedit.github.io "一键部署")
这一步很简单,一路下一步,确定即可

### 绑定域名
![](https://i.loli.net/2021/01/19/3jWHA6GeOLq1YJn.png)
## 注册本站

用github直接登录本站,享受在线管理文章的乐趣



## 简单瞅一眼本站[帮助文档](https://jing.gezhong.vip/help.html "帮助文档")

重点看一眼 设置部分，这一部分很强大，很强，强！
增加、删除，编辑、保存，发布 全部在本站操作即可


# 部署到Velcel
[![部署到vercel](https://vercel.com/button "部署到vercel")](https://vercel.com/import/project?template=https://github.com/jingtaiboke/jingtaiboke.github.io "部署到vercel")

settings--->git-->Ignored Build Step

	git diff --quiet HEAD^ HEAD README.md
	
	

# 使用 Travis Ci自动部署到github pages
GH_TOKEN
.travis.yml
```
sudo: false
language: node_js
node_js:
  - 10 # use nodejs v10 LTS
cache: npm
branches:
  only:
    - master # build master branch only
script:
  - hexo generate # generate static files
deploy:
  provider: pages
  skip-cleanup: true
  github-token: $GH_TOKEN
  keep-history: true
  on:
    branch: master
  local-dir: public
```

## 修改page的分支为`gh-pages`