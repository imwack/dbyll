---
layout: post
title: "String 类学习笔记 - 1"
date: 2017-01-22 21:34
author: imwack
comments: true
categories: [C++, string]
tags: []
---
从今天开始看一下C++ STL函数库。之前一直没看，时间不多了，从string开始看起

**1.构造函数~**

下列是常见的构造函数


<code class=""> 1.    string(const char*)
           string str("hello string");
    
     2.    string(size_type n,char c)    //初始化n个字符为c
         string str(10,'c');
    
     3.    string(const string &amp;s)
         string a("hello");
         string b(a);    //用另一个string初始化
    
     4.    string()
    
     5.    string(const char* s,size_type n)    //初始化为s字符串指向的前n个
    
     6.     string(Iter begin,Iter end)        //初始化为迭代器[begin , end)
    
     7.    string(const string &amp;str,size_type pos=0,size_type n=pos)
         //初始化为字符串str从pos开始的n个字符`</pre>
    **2.运算重载**
    <pre class="pure-highlightjs"><code class="">//加法
        string a ,b;
        string c = a+b;
        c+= "Oops";
    
    //比较
        string a ,b ;
        a&lt;b;    a&gt;b;    a==b;
    
    //长度 size和length是一样的
        str.size();
        str.length();`

&nbsp;

&nbsp;
