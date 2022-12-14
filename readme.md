# 我的博客

# 1.前期准备

- 安装git:https://git-scm.com/download/win
- 安装node:https://nodejs.org/en/
- 安装cnpm:`npm install -g cnpm --registry==https://registry.npm.taobao.org`
- 安装hexo:`cnpm install -g hexo-cli`
- 生成.ssh密钥：`ssh-keygen -t rsa -C "你的github登录邮箱"`
- 把公共密码复制到github上： `C:\Users\您的用户名\.ssh\id_rsa.pub`的内容复制到` github 主页，进入个人设置 -> SSH and GPG keys -> New SSH key`
- 配置user和email:`git config --global user.name "您的 Github username"`和`git config --global user.email "xxx@qq.com"`


# 2.使用 Typora 编写博客
## 2.1 Typora 介绍
Typora 是一款轻便简洁的 Markdown 编辑器，支持即时渲染技术，这也是与其他 Markdown 编辑器最显著的区别。即时渲染使得你写Markdown 就像是写 Word 文档一样流畅自如，不像其他编辑器的有编辑栏和显示栏。

优点:

- 简洁美观

- 实时预览

- 扩展语法

- 跨平台

## 2.2 安装 Typora

地址: 「typora-setup-x64(1).exe」https://www.aliyundrive.com/s/1SQzr6JXeR8 点击链接保存，或者复制本段内容，打开「阿里云盘」APP ，无需下载极速在线查看，视频原画倍速播放。

## 2.3 写博客

1、在 `D:\hexo` 目录下，通过输入命令: `hexo new "文章 title"` 会在` /source `文件夹下生成对应文章的` .md 文件`，然后就可以通过` Typora `打开此文件编写文章并保存了

2、当您写完该篇文章后，依次输入以下命令生成文章:

- `hexo clean` ：删除 public 文件夹，即删除旧的博客文章

- `hexo g`     ：生成 public 文件夹，即生成新的博客文章相关 html 文件

- `hexo s`     ：本地查看

- `hexo d`     ：将博客推送到 github 上的master

另外需要以下命令把本次更新的部署资源推到hexo
- git add .
- git commit -m "update"
- git push -u hexo hexo:hexo



## 其他 

向 Hexo 博客中插入图片

当 Hexo 项目中只用到少量图片时，可以将图片统一放在 source/images 文件夹中，通过 markdown 语法访问它们。
```md
![可以写关于图片的描述](/images/image.jpg)
```
图片既可以在首页内容中访问到，也可以在文章正文中访问到。
