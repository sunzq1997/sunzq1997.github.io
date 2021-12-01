---
title: "Maven修改阿里云镜像"
date: 2021-12-01T19:18:14+08:00
draft: true
---

1. config.xml中添加如下
```xml
    <mirror>   
         <id>aliyunmaven</id>
         <mirrorOf>*</mirrorOf>
         <name>阿里云公共仓库</name>       
         <url>https://maven.aliyun.com/repository/public</url>
   </mirror>

```
2. idea中添加如下
```bash
-Dmaven.wagon.http.ssl.insecure=true -Dmaven.wagon.http.ssl.allowall=true
```
![](https://cdn.jsdelivr.net/gh/sunzq1997/pic@main/uPic/Snipaste_2021-11-25_08-34-12.png)
