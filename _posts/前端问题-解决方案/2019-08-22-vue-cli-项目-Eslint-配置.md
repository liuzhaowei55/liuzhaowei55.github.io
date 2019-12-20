---
layout: post
title: vue-cli 项目 Eslint 配置
date: 2019-08-22 13:49:23
updated: 2019-08-22 13:49:23
permalink: /1566453043
categories:
tags:
---

## eslint-plugin-vue

主页：[https://eslint.vuejs.org/](https://eslint.vuejs.org/)

这个项目为所有的 `vue` 项目提供了统一的渐进的风格指南，我强烈推荐 `vue` 项目统一使用该样式。

## .eslintrc.js

```javascript
module.exports = {
  root: true,
  env: {
    node: true
  },
  extends: ["plugin:vue/essential", "@vue/prettier"],
  rules: {
    "no-console": process.env.NODE_ENV === "production" ? "error" : "off",
    "no-debugger": process.env.NODE_ENV === "production" ? "error" : "off"
  },
  parserOptions: {
    parser: "babel-eslint"
  }
};
```

## .prettierrc.js

``` javascript
module.exports = {
  printWidth: 120
};

```