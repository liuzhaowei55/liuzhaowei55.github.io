---
title: 在 Docker 中运行 cron
categories:
  - Docker
id: 1536223372
---

```yml
version: "3.3"

services:
  cron:
    restart: always
    image: alpine
    command: crond -f
```

很简单，其实就是要把 cron 服务放到前台来运行，不然会容器运行完会退出 