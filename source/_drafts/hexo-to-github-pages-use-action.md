> 本文讲述,使用github action 自动部署hexo静态博客到github pages


# 准备参数
 ## git地址:
 打开你的博客repo网址例如: https://github.com/jingtaiboke/jingtaiboke.github.io
 分别点击 code-->ssh-->复制这个地址:
 ```
 git@github.com:jingtaiboke/jingtaiboke.github.io.git
 ```
 ![](https://i.loli.net/2021/01/21/kuX9NgsxQ6S2hUi.png)
 
 
 ## SSH KEY
 你需要用命令行生成一一对ssh-keygen
 ```
 ssh-keygen -t rsa -b 4096 -f ~/.ssh/github-actions-deploy
 ```
 
 来到 https://github.com/settings/keys 添加ssh key