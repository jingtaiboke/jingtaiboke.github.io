---
title: 这可能是最简单的markdown静态站点生成器了
permalink: simple-markdown-site.html
cover: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/af0d1a2f-a35b-454a-8f96-86d4f9fedebb.png
updated: 2021-03-03 12:04:20
date: 2021-03-03 12:04:20
categories: 
- [静态博客技术]

tags: 
- 静态站点
- markdown
- 生成器
- html
- 最简单
---


> 这可能是史上最简单的静态站点生成器了,使用markdown作为源文件,生成html静态站点,并且是渲染过的


## 只有3个文件夹

1. posts:`存放markdown文件`

2. template : `模板文件`

3. public : `html发布文件`

## 使用方法:

```
git clone https://github.com/jingtaiboke/simple-markdown-site
cd simple-markdown-site
npm i
npm run build

```

## 用到的库

* markdown-styles

## 一键部署到vercel

 [![一键部署hexo到vercel](https://vercel.com/button "一键部署到vercel")](https://vercel.com/import/project?template=https://github.com/jingtaiboke/simple-markdown-site "一键部署到vercel")
## 演示

[DEMO](https://heji.vercel.app/ "demo")

![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/678b1e57-6abb-45d7-8771-a46e9b922258.png)

## 推荐几个类似的

###  https://docsify.js.org/

 > 直接加载md文件,无渲染,搜索引擎不友好,至少百度不友好 [demo](https://github.com/docsifyjs/docsify "free-for.dev")

### https://github.com/jingtaiboke/artless

> 同上 无渲染 [demo](https://artless-wxlzmt.netlify.app/ "demo")

### https://github.com/me1a/mini-book

> 有渲染,node构建,首页直接是个搜索框








