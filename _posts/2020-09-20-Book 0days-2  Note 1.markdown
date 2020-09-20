---
layout:     post
title:      "Book 0days-2  Note 1"
subtitle:   " \"Information Security\""
date:       2020-09-20 14:47:00
author:     "Nastul"
header-img: "img/data-featured-image-1.jpg"
tags:
    - InformationSecurity  
---

### **Basic knowledge**

由于最近研究方向需要，找了些安全相关的书看，网上好像推荐0day这本书比较多，就写个笔记记录下。

ollydbg et al. 动态调试工具， IDA 静态反汇编工具



bug：功能性逻辑缺陷

漏洞：安全性逻辑权限

对于非可执行文件， 如果文件在解析时存在某些漏洞，比如说缓冲区溢出，就有可能导致该文件的恶意代码被执行。

- 漏洞挖掘- 安全性漏洞通常不会对软件功能本身造成很大影响，所以很难被QA工程师的功能性测试发现。需要进行Penetration test（攻击测试）， by Tiger team 或者 Ethic hacker。学术界主要是静态分析寻找源代码中的漏洞， 工业界普遍的采用Fuzzing。 灰盒测试

- 分析漏洞 搜索到 POC（proof of concept）重现漏洞被触发的场景。使用调试器观察漏洞细节，或者利用工具 Paimei 等。如果没有POC 通用的方法是使用补丁比较器，  然后利用反汇编工具IDA Pro 重点逆向分析该位置。

- 漏洞利用

未被修复未被公布的常常叫做 0day 漏洞。



### 二进制文件

PE（Portable Exec utable）是 Win32 平台下可执行文件. （如“*.exe”文件和“*.dll”文件）都是典型的 PE 文件。











