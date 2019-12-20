---
layout: post
title: "field injection is not recommended"
date: 2019-11-01 14:45:04
updated: 2019-11-01 14:45:04
categories: 
  - SpringBoot
tags: 
  - java
  - SpringBoot
---

在 spring boot 开发中，如果你使用了 `@Autowired` 注解来注入多态对象可能会收获一个提示：

> field injection is not recommended

这个提示并不影响程序的正常运行，只是使用了一些不太建议的编码方式。

这里有一篇文章，很好的说明了这个问题，以及该怎么去解决这个问题。

[Field Dependency Injection Considered Harmful](https://www.vojtechruzicka.com/field-dependency-injection-considered-harmful/)