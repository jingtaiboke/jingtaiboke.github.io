# 简介

> 本文主角:[静态博客编辑器](https://jingtaiboke.com/ "静态博客编辑器")

## 首先,[这是一个github内容编辑器](https://jingtaiboke.com/ "这是一个github内容编辑器")
可以方便的增加,删除,编辑github文件
markdown文件还支持实时预览

## 期次,主要定位是[静态博客文章管理](https://jingtaiboke.com/ "静态博客文章管理")


支持Hexo、Hugo、jekyll等主流静态博客
并且根据静态博客特点做了很多优化,使大家专注于写文章,而不是折腾什么博客,内容才是王道


# 快速上手,5分钟毕业

> 如果你只是想建个博客,写写文章,看完这一节就毕业了,其他的一概不用看
避免选择恐惧症,这里只介绍一条路,这条路就是

`github+hexo+netlify`


## 注册github
首先你要有一个[https://github.com/](https://github.com/ "https://github.com/")

## 一键部署到netlify

[![一键部署](https://d33wubrfki0l68.cloudfront.net/65a18ef24e011fbc0b5ddb411d611c0e1d1111a6/17e0b/images/deploy-button.svg "一键部署")](https://app.netlify.com/start/deploy?repository=https://github.com/jingtaiboke/jingtaiboke.github.io "一键部署")
这一步很简单,一路下一步,确定即可

### 绑定域名
![](https://i.loli.net/2021/01/20/Vwx52bKog6cujap.png)

## 登录本站

用github直接登录本站,享受在线管理文章的乐趣

>授权的时候可以自己选择 是否包含**私有库**,看你需求,无授权当然无法管理私有库


## 帮助文档

### 这是操作界面
增加、删除，编辑、保存，发布 全部在本站操作即可
![](https://s3.ax1x.com/2021/01/20/sWzOyD.png)

### 图床方案

#### 一. 直接截图粘贴

> 微信截图,QQ截图.其他各种截图工具 Ctrl+V后,自动上传到sm.ms图床

#### 二.本地文件拖拽

> 从电脑文件管理器,直接拖拽到编辑器,自动上传到sm.ms图床

#### 三.网络图片粘贴

> 右键网页图片-->复制-->来到编辑区Ctrl+V,自动上传到sm.ms图床

#### 四.Chevereto系列图床

本站已经集成Chevereto图床插件,此系列的图床,可以使用插件方式上传
当然可以设置成自己的图床
默认使用https://imgchr.com/
[更多Chevereto图床](https://github.com/Chevereto/api#-powered-by-chevereto "更多Chevereto图床")
![](https://i.loli.net/2021/01/20/96YuCBjfl5WtMmo.png)

### [设置](https://jingtaiboke.com/config.php "设置")

#### 1.个人网站设置

> 设置的网站,会显示在本站首页用户区,未使用本站服务的请不要设置,有封号风险

#### 2.仓库设置(Repository)

> 设置需要本站操作的`Repository`,支持多个,用英文逗号隔开
例如:`myblogA,myblogB`

#### 3.其他设置

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

![](https://i.loli.net/2021/01/20/LQBJGxAwZ8jHubs.png)
* 2021-01-20 19:56:47
* 2021-01-20 20:02:58
* 2021-01-20 20:11:15
* 2021-01-20 20:19:19
* 2021-01-20 20:20:08
* 2021-01-20 20:30:38
* 2021-01-21 08:49:35
* 2021-01-21 10:56:44
* 2021-01-25 00:05:13
* 2021-01-25 00:17:33
* 2021-01-25 00:19:01
* 2021-01-25 00:20:30
* 2021-01-25 00:28:23
* 2021-01-25 00:30:43
* 2021-01-25 00:35:01
* 2021-02-08 14:53:26
* 2021-02-09 17:18:17
* 2021-02-09 17:23:14
* 2021-02-09 17:58:35
* 2021-02-12 15:17:20
* 2021-02-19 09:55:15
* 2021-02-19 09:57:26
* 2021-02-19 10:06:15
* 2021-02-19 10:39:40