---
layout:     post
title:      java中的“==”与equals的区别
subtitle:   java中的“==”与equals的区别
date:       2017-12-9
author:     Mr.Li
header-img: 
catalog: true
tags:
    - java
---
 # 区别
  “==”使用比equals（）更加广泛，equals只能用于String类型的
  
    ```
    int a;
    a.equals();//没有此方法
    String a；
    a.equals(参数)；//有此方法
    ```
    
  _**其次对于两个引用型变量，必须指向同一对象时候，才能返回true，而equals则只要两个字符串序列相同，就返回true**
  
    ```
    String str1 = new String("hello");
    String str2 = new String("hello");
    str1==str2;//返回false
    str1.equals(str2);//返回true
    
    ```
