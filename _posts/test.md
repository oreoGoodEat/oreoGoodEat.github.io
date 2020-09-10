---
layout: page
title: "This post demonstrates post content styles"
subtitle: "This is a subtitle"
date:   2016-05-20 21:21:21 +0530
categories: junk
author: "Bart Simpson"
meta: "Springfield"
---

# 搭建个人技术博客

> 使用GitHub Pages + Jekyll 快速部署个人博客

> - GitHub Pages 
>       - 定义：给所有个人注册用户提供一个个人主页
>       - 如何访问个人域名:用户名.github.io
>       - 如何编写主页：建立一个域名为项目名的远程版本仓库，只需要向该远程版本仓库中的master分支提交代码即可
> - Jekyll（该代码中必须要有一个文件为index.html）
>       - 定义：可以将markdow语法自动编译成HTML语法的一个工具
>       - 安装：不需要自己安装，在GitHub网站中预安装的
>       - 使用：不需要人为使用，当请求个人域名时，GitHub服务器会读取仓库（以个人域名命名的远程版本仓库）中master分支中的代码，如果该代码为markdow语法会自动调用Jekyll，将其编译为HTML并返回客户端

 - 建立一个以个人域名为项目名的远程版本仓库
 - 访问一个主题网址：http://jekyllthemes.org/ ，选择一个主题，将其代码复制至我们的仓库中的master分支中
 - 以上两步可以合为一步，在主题仓库中点击fork，点击setting设置仓库名即可
	 - 将远程版本库中的代码克隆到本地
	 - 点击code，复制链接
	 - 在文件打开终端执行克隆，git clone -b master https://github.com/oreoGoodEat/oreoGoodEat.github.io.git myBlog 
	 - 从远程版本仓库中克隆下来的代码会自动创建本地版本仓库
 - 将远程版本库的代码克隆到本地
 - 修改配置文件以及页面内容
 - 书写博客

# github 指令
- git init  初始化本地仓库（建立.git 文件夹）
- git status 查看本地版本库状态 ，分为暂存区和本地库（查看代码是否提交）若提交至本地则显示“xxxclean”
- git add .   . 表示当前文件夹所有内容
- git commit -m "备注信息"  
- git config
- git clone -b master https
- git push 推送链接 master:master
- 合并远程分支：本地版本库必须与远程版本库一致
 
# 网络请求
 
 - 完整url：协议 + 域名 + 端口 + 文件路径 + 参数
 - 协议：http https ws wss ftp sftp .... 客户端与服务端双方约定的一种处理请求方式的方式
 	- 客户端：发送请求的软件（浏览器，调用电脑的网络模块（网卡驱动））
 	- 服务端：处理请求的软件（webServer：apache ）
 	- 约定的内容：发送 接受 处理请求的方式
 - 域名：IP的别名
	- 前缀（主域名） 名字 后缀：www.baidu.com
 	- 映射关系：一对一
 	- host文件中寻找域名与IP的映射关系 
 	- 在本地hosts中写的IP和域名的映射关系称为静态路由（C:\Windows\System32\drivers\etc> notepad.exe hosts）
 	- 本地域名解析
 	- dns域名解析 dns服务器
 - 端口
 - 文件路径
 - 参数

