---
layout:     post
title:      java中的继承
subtitle:   继承
date:       2017-12-8
author:     Mr.Li
header-img: 
catalog: true
tags:
    - java
---

# public private protected 说明
 private主要是不要子类直接访问父类的Field；protected主要是某个方法被重写，可以用protected修饰
 
# 初始化模块
 在创建java对象时候隐式执行，而且是在执行构造器之前执行，只能用static进行修饰，用static修饰的是静态初始化，而不是在创建对象时候才执行，类初始化阶段执行初始化
 
# 增加的包装类
java里int是单独拿出来定义的，没有tostring（）方法，java的int是单独定义的，其实这也是java的一个缺点，java靠的是包装类Integer来实现调用toString（）这一方法的

_**所有java对象都是Object类的实例，都可以直接调用该类中定义的方法，虽有java类都是object的子类
 **
