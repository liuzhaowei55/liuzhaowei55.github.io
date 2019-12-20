---
title: vscode-php开发配置
categories: 
- 安装配置
---

> 前提：开发机已经安装了 PHP 和 [`composer`](https://getcomposer.org/)

1. 安装 [`phpcs`](https://github.com/squizlabs/PHP_CodeSniffer)，
```bash
composer global require "squizlabs/php_codesniffer"
```
2. 安装 [`php-cs-fixer`](https://github.com/FriendsOfPhp/PHP-CS-Fixer)
```bash
composer global require "friendsofphp/php-cs-fixer"
```
3.安装以下拓展

* [php-cs-fixer](https://marketplace.visualstudio.com/items?itemName=junstyle.php-cs-fixer)
* [phpcs](https://marketplace.visualstudio.com/items?itemName=ikappas.phpcs)
* [php-docblocker](https://marketplace.visualstudio.com/items?itemName=neilbrayfield.php-docblocker)
* [crane](https://marketplace.visualstudio.com/items?itemName=HvyIndustries.crane)