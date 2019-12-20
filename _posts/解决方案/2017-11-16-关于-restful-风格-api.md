---
title: 关于-restful-风格-api
categries: 
- 解决方案
---
下边的这些都还只是想法，自己也还没有完全安装这个风格来做，至于为什么不在 URL 中添加 `/:id` 这样的匹配字段是因为，这样虽然看起来很好，但是这是开发不友好的，最近在用 Golang 开发的时候，像这种 `params` 都没有办法优雅的添加到 URL 中，只能用字符串拼接的方式来做，所以我更加推荐用 `query` 这种比较正统的传参方式来做。
欢迎大家在公众号中回复我。

|method|url|des|
|---|---|---|
|POST|HOST/user/new|创建|
|GET|HOST/user/index|列表|
|GET|HOST/user/show|对象|
|DELETE|HOST/user/delete|删除|
|PATCH|HOST/user/update|更新|