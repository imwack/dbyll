---
layout: post
title: "35.第一个只出现一次的字符位置"
date: 2017-01-21 15:16
author: imwack
comments: true
categories: [剑指offer]
tags: []
---
<h2 class="subject-item-title">题目描述


<div class="subject-describe">在一个字符串(1&lt;=字符串长度&lt;=10000，全部由大写字母组成)中找到第一个只出现一次的字符,并返回它的位置</div>
<div class="subject-describe">
<h2 class="subject-item-title">题目解答


</div>
<div class="subject-describe">首先想到的是哈希表计算次数O(n)、其次是排序O(n logn)</div>
<div class="subject-describe">因为是字符 直接开数组作为计数，下标为字符对应的ASCII码</div>
<div class="subject-describe">


<code class="">    int FirstNotRepeatingChar(string str) {
    
            int *count = new int[1024];
            int index;
            for(int i=0;i&lt;str.length();i++)
                count[str[i]]++;
    
                
            for(int i=0;i&lt;str.length();i++){
                if(count[str[i]]==1){
                   return i;
                }
            }
            return -1;
        }`

&nbsp;

</div>
