---
layout: post
title: HTML To Canvas & Canvas To Image
categories:
  - 前端问题-解决方案
id: 1536223575
---

今天在做项目时遇到一个问题：用 JS 保存 dom 为图片保存在本地，中间遇到了一点问题，这里记录下来。

第一步，把 dom 转为 canvas 对象，这里使用的是 [html2canvas](https://html2canvas.hertzen.com/)

```javascript
html2canvas(document.body).then( (canvas)=> {
          
})
```

第二步，把 canvas 对象转为图片下载，这里稍微遇到一些曲折，略去不说，下边是解决办法

```javascript
html2canvas(document.body).then( (canvas)=> {
        // canvas 对象转为 base64 对象ß
        var imgUri = canvas.toDataURL('image/png')
        // js 生成一个 a dom 节点，然后模拟点击，让它下载
        var a = document.createElement('a')
        a.setAttribute('href', imgUri)
        a.setAttribute('download', 'download.png')
        a.click()
})
```