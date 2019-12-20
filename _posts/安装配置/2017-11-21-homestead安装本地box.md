---
layout: post
title: Homestead 安装本地 box
categories: 
  - 安装配置
---

新建一个如下的 `metadata.json` 文件，然后编辑版本和文件位置，正常添加即可。
```json
{
    "name": "laravel/homestead",
    "versions": [
    {
        "version": "3.0.0",
        "providers": [
        {
            "name": "virtualbox",
            "url": "file:///Users/where/Downloads/efd18095-ab30-4e39-ad54-f317d33212bb"
        }]
    }]
}
```