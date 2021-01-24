---
title: 静态博客编辑器-系列教程(一)  快速入门
date: 2021-01-20 19:19:14
categories: 
- [系列教程]

tags: 
- 静态博客编辑器
- 教程

permalink: help1.html
cover: https://s3.ax1x.com/2021/01/20/sf9SRP.png
updated: 2021-01-20 19:19:14

---
# 简介

> [静态博客编辑器](https://jingtaiboke.com/ "静态博客编辑器")
是一个静态博客在线写作工具,脱离命令行,所见即所得,方便的图床管理
支持Hexo、Hugo、jekyll等主流静态博客
根据静态博客特点做了很多优化,使大家专注于写文章,而不是折腾什么博客,内容才是王道

# 使用guthub登录

用github直接登录本站,享受在线管理文章的乐趣
在这里写上你需要本站管理的仓库,多个可以用逗号隔开(英文逗号)

![](https://img.youzibe.com/upload/2021/01/242358-1611503954756.png)

# 帮助文档

## 操作界面
增加、删除，编辑、保存，发布 全部在本站操作即可

![](https://img.youzibe.com/upload/2021/01/242342-1611502941620.png)


## 新建文章

* 点击文件夹后面的+号

* 选中刚才新建的文件,在右侧改文件名

![](https://img.youzibe.com/upload/2021/01/242349-1611503365433.png)

## 删除文章

* 点击文件名后面的小按钮,即可删除(从github仓库删除)
![](https://img.youzibe.com/upload/2021/01/242350-1611503471577.png)

## 文件重命名

* 点击需要改名的文件,在右侧直接改名,会复制一个新文件

* 不要忘了删除旧文件

## 搜索文件

这里是搜索框,只支持打开过的文件夹,未加载的不会搜索
![](https://img.youzibe.com/upload/2021/01/242354-1611503714683.png)



## 图床方案

### 一. 直接截图粘贴

> 微信截图,QQ截图.其他各种工具截图 Ctrl+V后,自动上传到sm.ms图床,并插入文章

### 二. 本地文件拖拽

> 从电脑文件管理器,直接拖拽到编辑器,自动上传到sm.ms图床

### 三. 网络图片粘贴

> 右键网页图片-->复制-->来到编辑区Ctrl+V,自动上传到sm.ms图床

### 四.Chevereto系列图床

本站已经集成Chevereto图床插件,此系列的图床,可以使用插件方式上传
当然可以设置成自己的图床
默认使用https://imgchr.com/
[更多Chevereto图床](https://github.com/Chevereto/api#-powered-by-chevereto "更多Chevereto图床")
![](https://img.youzibe.com/upload/2021/01/242355-1611503757695.png)

### 五. 自定义图床API

支持各种自定义api,比如站长使用的u-file来存储图片,有需要可以联系我

## [设置](https://jingtaiboke.com/config.php "设置")

### 1.个人网站设置

> 设置的网站,会显示在本站首页用户区,未使用本站服务的请不要设置,有封号风险

### 2.仓库设置(Repository)

> 设置需要本站操作的`Repository`,支持多个,用英文逗号隔开
例如:`myblogA,myblogB`

### 3.其他设置

> 其他设置太杂,全部放在一起,反而干净了,必须使用标准json格式
* lei: 分类设置(~~英文单词太长,记不住~~)
* tags: 标签
* links:将显示为**常用链接**
* smmsToken : sm.ms图床token(截图粘贴用,默认用公共API)
* cheveretoPicBed : chevereto图床网址,默认"https://imgchr.com"
* frontMatter : 文章头模板,用于一键插入博客头,名字,内容都可随便设置,其中{now}为变量=现在时间

```
{
	"lei": [
		"[系列教程]",
		"[编辑器相关]",
		"[静态博客技术]"
	],
	"tags": ["静态博客", "编辑器", "hexo", "hugo","jekyll","vercel","Netlify"],
	"links": [{
			"title": "请去",
			"url": "/config.php"
		},
		{
			"title": "后台",
			"url": "/config.php"
		},
		{
			"title": "设置",
			"url": "/config.php"
		}
	],
	"smmsToken": "",
	"cheveretoPicBed": "https://imgchr.com",
	"frontMatter": {
		"MyHexo": ["---",
			"title: hexo post",
			"permalink: ",
			"cover: ",
			"updated: {now}",
			"date: {now}",
			"categories: ",
			"tags: ",
			"---"
		],
		"MyHugo": ["---",
			"title: hugo post",
			"date: {now}",
			"categories: ",
			"tags: ",
			"---"
		],
		"MySelf": ["---",
			"title: my self  post",
			"date: {now}",
			"categories: ",
			"tags: ",
			"---"
		]
	}
}
```

![](https://img.youzibe.com/upload/2021/01/250000-1611504047197.png)
