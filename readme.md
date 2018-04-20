# PHP Memcache 扩展

PHP 5.2 - 5.6

供windows使用的PHP Memcache扩展包(.dll)

> php5.2以下版本使用memcached-client-php

# 如何选择

参考下图

![如何选择](https://raw.githubusercontent.com/GHBJayce/php_memcache_windows/master/assets/how%20to%20choose.jpg)


# 如何使用

## 步骤一 加入php扩展

找到`php\ext\`，将下载好的扩展放到这个目录下
![php\ext](https://raw.githubusercontent.com/GHBJayce/php_memcache_windows/master/assets/php%20ext%20dir.jpg)

接着，编辑`php\php.ini`，在最后一行加入如下代码

```
extension=php_memcache.dll
```

> 其中`php_memcache.dll`要替换成实际的名称

![php\php.ini](https://raw.githubusercontent.com/GHBJayce/php_memcache_windows/master/assets/php.ini.jpg)

然后重启服务，查看`phpinfo()`，`Ctrl + F`搜索`memcache`。

![memcache](https://raw.githubusercontent.com/GHBJayce/php_memcache_windows/master/assets/memcache.jpg)


## 步骤二 启动服务

在下载好的包中找到`memcached\memcached-1.4.5-x`，根据自己环境选择工具。然后启动服务

![run Memcached server](https://raw.githubusercontent.com/GHBJayce/php_memcache_windows/master/assets/run%20memcached%20server.jpg)


## 代码使用

[php.net Memcache](http://php.net/manual/en/book.memcache.php)
