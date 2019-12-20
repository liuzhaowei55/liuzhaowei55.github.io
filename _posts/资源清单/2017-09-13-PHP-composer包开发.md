---
title: composer 包开发
categories:
- 资源清单
---


Demo：[https://github.com/liuzhaowei55/accessyou](https://github.com/liuzhaowei55/accessyou)
这是一个香港通知短信下发的库

如何导入本地库：

```json
{
    "require": {
        "moorper/accessyou": "^1.0"
    },
    "repositories": [
        {
            "type": "path",
            "url": "packages/accessyou"//相对于composer.json的包位置
        }
    ]
}
```


