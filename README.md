# Emby劫持API进行认证方法

简介：

​	这个东西的本质就是创造一个CA证书，然后用CA证书自签一个`mb3admin.com`网站。接着用NGINX默认返回固定的值。



1、Nginx配置已经放在目录

2、Emby所在的服务器需要导入CA证书，如果是Emby的官方Docker的话，需要把文件拷贝到`/etc/ssl/cert`目录内，完成以后重启即可。

3、HOST方面，可以在路由器，HOSTNAME等方面入手，方法很多，不在赘述。
