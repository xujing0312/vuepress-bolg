# 如何理解作用域链和闭包

红宝书(p178)上对于闭包的定义：`闭包是指有权访问另外一个函数内部的私有变量`,所以有两个特点

* 是一个函数

* 能访问另外一个函数的私有变量

## 闭包总结

总结: 闭包就是一个函数引用另外一个函数的变量,因为变量被引用也就不会被回收,因此可以用来封装一个私有变量

## 什么是作用域链?

**作用域链**: 当访问一个变量的时候,解释器首先会在当前的作用域去寻找标识符,如果没有找到,就会找父级的作用域,直到找到该作用域链或作用域中,我们称之为作用域链
