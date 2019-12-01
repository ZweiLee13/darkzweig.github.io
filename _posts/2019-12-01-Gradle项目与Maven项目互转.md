---
layout:     post
title:      "Gradle项目与Maven项目互转"
subtitle:   "\"笔记\""
date:       2019-12-1 19:57:30
author:     "Zweig"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
- 笔记
- gradle
- maven
- code
```
在build.gradle中增加以下内容
···java
apply plugin: 'maven'
```
在Gradle项目根目录下执行 gradle install，我们会发现根目录的build文件夹下生成了一个poms文件夹里面有pom-default.xml文件。把它复制到根目录下，改名成pom.xml即可