---
title: wordpress文章导入语雀脚本-python
permalink: wordpress-import-to-yuque.html
cover: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/a93fd674-8bc3-426e-af9f-b2ff128c3125.png
updated: 2021-03-08 12:50:00
date: 2021-03-08 12:50:00
categories: 
- [静态博客技术]

tags: 
- 博客
- 语雀
- 导入
- wordpress

---

> 语雀很适合做个人博客,尤其是隐私博客,将wordpress文章导入到语雀方法如下

## 1.首先[注册语雀(含邀请链接)](https://www.yuque.com/login?platform=wechat&inviteToken=6f77531ad0334e1991ac5c8b18609acc163341dcdabfa632c2c430d6d091579c)

## 2.从wordpress数据库导出为html文件

导入的时候,用文件名作为语雀文章标题
python脚本在这里下载:
[语雀团队域名-扫描脚本.py](https://545c.com/f/19473836-484864849-27fa0c)
（访问密码：2233）

## 将生成的html打包成zip文件

我是在根目录打包的,也就是压缩包内没有文件夹,直接全部html文件

## 3.导入语雀

### 导入

`新建`-->`导入`-->`HTML or Markdown.zip`

然后务必选中最后一项(防止标题乱码)

![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/3d46d02a-8013-4df0-9fa6-22a5cd175ff9.png)

![](https://vkceyugu.cdn.bspapp.com/VKCEYUGU-3c98b21f-9e7e-4bcb-9142-940554115122/a93fd674-8bc3-426e-af9f-b2ff128c3125.png)

### 然后就是下一步了

首发自:[https://www.jingtaiboke.com/wordpress-import-to-yuque.html](https://www.jingtaiboke.com/wordpress-import-to-yuque.html)