---
layout:     post
title:      ubuntu
subtitle:   ubuntu文件夹操作
date:       2017-12-12
author:     BY
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - ubuntu
---

# Ubuntu下修改目录权限命令如下：
chmod 600 name （只有所有者有读和写的权限）
chmod 644 name （所有者有读和写的权限，组用户只有读的权限）
chmod 700 name （只有所有者有读和写以及执行的权限）
chmod 666 name （每个人都有读和写的权限）
chmod 777 name （每个人都有读和写以及执行的权限）

修改文件夹：sudo rm -r tomcat

 # Ubuntu下创建、重命名、删除文件及文件夹，
mkdir 目录名 ——创建一个目录
rmdir 空目录名 ——删除一个空目录
rm 文件名 文件名 ——删除一个文件或多个文件
rm -rf 非空目录名 ——删除一个非空目录下的一切
touch 文件名 ——创建一个空文件

重命名文件（夹） / 移动文件（夹）到指定文件夹
执行格式： mv source destination


 # 关于LINUX权限-bash: ./startup.sh: Permission denied
<script type="text/javascript"></script><script type="text/javascript"></script>
在执行./startup.sh,或者./shutdown.sh的时候，爆出了Permission denied，
其实很简单，就是今天在执行tomcat的时候，用户没有权限，而导致无法执行，
用命令chmod 修改一下bin目录下的.sh权限就可以了
如chmod u+x *.sh

# 腾讯云服务器Java+Tomcat+Mysql环境搭建
http://www.jianshu.com/p/e59ae18638f5
