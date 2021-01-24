---
title: 3分钟搭建Hexo静态博客-(vercel篇)
date: 2021-01-24 20:37:43
categories: 
- [系列教程]

tags: 
- 静态博客编辑器
- hexo
- vercel


permalink: build-hexo.html
cover: https://s3.ax1x.com/2021/01/20/sf9SRP.png
updated: 2021-01-20 19:19:14

---
# 前言
> 静态博客有些复杂,太折腾,有些人搞不明白,望而却步,本文让你零基础搭建静态博客,快速上手,而且在线写博客,不用懂命令行

# 用到的工具

* [github](https://github.com/ "github") 存放静态博客程序,本文使用hexo
* [Vercel](https://vercel.com/ "Vercel") 傻瓜式ci部署 + 网站托管 + 绑定域名
* [静态博客编辑器](https://jingtaiboke.com/ "静态博客编辑器") 在线写hexo博客,不用命令行

# 第一步:一键部署静态博客

点击这个按钮,一键部署 [![一键部署hexo到vercel](https://vercel.com/button "一键部署hexo到vercel")](https://vercel.com/import/project?template=https://github.com/jingtaiboke/jingtaiboke.github.io "一键部署hexo到vercel")

## 界面1,随便取一个名字
![](http://img.youzibe.com/upload/2021/01/242316-1611501410216.png)

## 界面2,选择github,并建立连接

![](http://img.youzibe.com/upload/2021/01/242315-1611501356761.png)

## 界面3,选择给仓库取个名字
![](http://img.youzibe.com/upload/2021/01/242318-1611501530195.png)

## 界面4,直接点部署然后等待
![](http://img.youzibe.com/upload/2021/01/242319-1611501601875.png)

## 界面5,部署后进控制台
![](http://img.youzibe.com/upload/2021/01/242321-1611501686000.png)

## 在vercel设置一个参数
选择刚才部署的站点--> setting--> git--> Ignored Build Step 填上下面代码,然后保存
```
git diff --quiet HEAD^ HEAD README.md
```
![](http://img.youzibe.com/upload/2021/01/242323-1611501812338.png)


## 绑定自己的域名

> vercel提供了一个二级域名,喜欢的话可以直接用,也可以绑定自己的域名

![](http://img.youzibe.com/upload/2021/01/242326-1611502020822.png)

## 部署完毕

这时候你已经有了一个静态博客,回到github看一眼,vercel帮你创建了一个新仓库,名字是你在界面3自己取的,记下来

# 在线写博客

在线写hexo博客神器登场了, 用github账号登录[静态博客编辑器](https://jingtaiboke.com/ "静态博客编辑器"),即可在线写博客了

这里是[使用教程](https://www.jingtaiboke.com/help1.html "使用教程")
