---
title: Laravel 的远程服务器任务处理器 Envoy
categories:
  - Laravel
id: 1536223484
---

注：  

 * [Laravel 的远程服务器任务处理器 Envoy](http://d.laravel-china.org/docs/5.4/envoy)

 操作步骤：
 
 1. 安装 Envoy `composer global require "laravel/envoy=~1.0"`
 2. 编写配置文件 `Envoy.blade.php`
 
 ```php
@servers(['web' => ['user@192.168.1.1']])
@task('foo', ['on' => 'web'])
    ls -la
@endtask
 ```
 3. 运行 `envoy run deploy`

 至此结束，具体使用方法可以看官方文档。
