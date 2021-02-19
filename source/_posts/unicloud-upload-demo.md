---
title: 从零部署一个unicloud程序-以文件上传为例
permalink: unicloud-upload-demo.md
cover: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/b759df11-b1a2-4bf6-8a51-1770df4867eb.png
updated: 2021-02-19 17:11:12
date: 2021-02-19 17:11:12
categories: 
- [系列教程]

tags: 
- unicloud
- 阿里云cdn
- 图床


---

> 本文将从零部署一个基于阿里云免费cnd的文件上传程序,演示整个部署过程以及一些坑

## 准备工作

### 账号注册,以及实名认证

[https://uniapp.dcloud.net.cn/](https://uniapp.dcloud.net.cn/ "https://uniapp.dcloud.net.cn/")

### 演示源码下载

[下载：（密码2233）](https://545c.com/d/19473836-42522931-e58c84 "源码下载：（密码2233）")

下载后解压

### 开发环境下载

绿色软件,解压直接运行

请选 [App开发版（261.97M）](https://download1.dcloud.net.cn/download/HBuilderX.3.1.2.20210206.full.zip "App开发版（261.97M）"),不要那个小的

### 用编辑器打开源码

Ctrl+O,选择源码文件夹

## 开始部署

现在你的界面应该是这样的
![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/d965ea10-8772-4aba-9c46-1bbc2b947fc5.png)

### 创建云服务空间

右键`uniCloud`文件夹,选择创建云服务空间,选阿里云

### 关联云服务空间
右键`uniCloud`文件夹,选择关联云服务空间,选刚才创建的


### 开通前端托管

- web端,进入刚才创建的空间,点击"前端网页托管",
- 再点`开通`,稍等几秒钟
- 点`参数配置`,复制`默认域名`
 > 例如`static-02198a5f-6b42-463e-844f-acd44036e817.bspapp.com`

- 再点跨域配置,将刚才的默认域名加上,当然你可以绑定自己的备案域名

 > 这一步很重要,否则云函数不会执行

![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/41339487-7b40-4a67-b1e3-190e6799f275.png)
![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/242bc2bd-e187-4b0a-882e-6e6879b6f6b4.png)


### 上传部署

进入编辑器,选中左侧项目--> 点菜单`发行` --> 点`上传网站到服务器`

稍等片提示成功,竣工

![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/421e8f75-a4f6-4a03-9582-fcddc35351a0.png)

### unicloud的实际应用

[静态博客编辑器](https://jingtaiboke.com/ "静态博客编辑器"),是一个静态博客管理后台.
已经融合unicloud阿里云图片上传,使用方法很简单
> 截图 --> Ctrl+V 直接插入到文章中
> 右键复制网页图片 --> Ctrl+V 也是支持的

从此写静态博客又方便了不少

![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/34e56954-308c-42b4-9169-4f73f5b08cca.png)




