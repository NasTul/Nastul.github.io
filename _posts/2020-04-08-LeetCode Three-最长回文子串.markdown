---
layout:     post
title:      "LeetCode Three-最长回文子串"
subtitle:   " \"Algorithm\""
date:       2020-04-08 08:18:00
author:     "Nastul"
header-img: "img/c62118211cf7422e8534e259f2f92e5e.jpeg"
tags:
    - LeetCode 
---
**[最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/)**

特殊情况  abba也是，所以不能只考虑奇数个数的字符



**爆破**

找到字符串中所有大于等于2的子串，然后判断该子串是否是回文子串



**动规**

画一张表，横竖分别是需要判断的字符串，当s[l]==s[r]而且dp[l+1]==dp[r-1]的时候将dp[l] [r]赋值为True , 也就是判断左右字符串是否相等，判断左右字符串的前一个是否相等。



**中心扩撒**

直接从中间开始找回文，注意回文子串的奇偶



**马拉车**

字串的间隙加上#，包括首尾