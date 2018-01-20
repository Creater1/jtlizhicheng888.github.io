---
layout:     post
title:      structs
subtitle:    structs学习
date:       2018-1-20
author:     MR.Li
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - java
    - struct
---
# structs配置
 很简单，点击项目->open modul setting->facts->点击加structs，OK了
 
# structs配置文件
 在resouses下边新建structs.xml文件，配置一下，主要配置
    
## 说明 ##
     <package name="null" namespace="/" extends="struts-default">
        <action name="login" class="action.LoginAction" method="success">
            <result name="success">
                index.jsp
            </result>
        </action>
        <action name="show" class="action.AdminAction" method="showAdmin">
            <result name="showAdmin">show.jsp</result>
        </action>
    </package>
   
 name是在浏览器输入的url，class是对应的类，method是class里边的方法，对应方法返回的也是showaDmin，<result name="">里边的参数主要根据方法showAdmin()
 里边的返回参数来填写，不然会报错
