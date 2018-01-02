---
layout:     post
title:      生活杂想
subtitle:   生活咋想
date:       2017-12-15
author:     MR.Li
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - java
    - 生活
---
# SystemService
系统服务的工具：工具，文件处理，

javabean 实体化类 DAO数据库处理：专门操作数据库，做缓存（增删改查）  hibinety：对数据库映射  

# Properties类继承自Hashtable
在Java中，其配置文件常为.properties文件，格式为文本文件，文件的内容的格式是“键=值”的格式，文本注释信息可以用"#"来注释
#### **提供的方法**
它提供了几个主要的方法：

1． getProperty ( String key)，用指定的键在此属性列表中搜索属性。也就是通过参数 key ，得到 key 所对应的 value。

2． load ( InputStream inStream)，从输入流中读取属性列表（键和元素对）。通过对指定的文件（比如说上面的 test.properties 文件）进行装载来获取该文件中的所有键 - 值对。以供 getProperty ( String key) 来搜索。

3． setProperty ( String key, String value) ，调用 Hashtable 的方法 put 。他通过调用基类的put方法来设置 键 - 值对。

4． store ( OutputStream out, String comments)，以适合使用 load 方法加载到 Properties 表中的格式，将此 Properties 表中的属性列表（键和元素对）写入输出流。与 load 方法相反，该方法将键 - 值对写入到指定的文件中去。

5． clear ()，清除所有装载的 键 - 值对。该方法在基类中提供。

# 读取配置文件
            
            Properties props_r = new Properties();
            InputStreamReader in = new InputStreamReader(new FileInputStream(SystemServiceImp.class.getResource("/").toURI().getPath()+"SystemSet.properties"), "UTF-8");
		      	props_r.load(in);
			      in.close();
**读取方式注意**
path不以’/'开头时，默认是从此类所在的包下取资源；
path  以’/'开头时，则是从ClassPath根下获取
