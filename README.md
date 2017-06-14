# owncloud 在线实验环境

## 软件简介

ownCloud是一个自我托管的文件同步和共享服务器。它可以通过Web界面访问您的数据，同步客户端或WebDAV，同时提供一个平台，可以轻松地查看，同步和共享各种设备，而这些平台都可以控制。ownCloud的开放架构可以通过简单但功能强大的API扩展，适用于应用程序和插件，并可与任何存储一起使用。

所属类别是服务器软件

## 软件官网

https://owncloud.org/

## Dockerfile 使用方法

### 启动owncloud
启动在端口80上侦听的ownCloud 8.1实例与以下一样简单：
```
$ docker run -d -p 80:80 owncloud:8.1
```
然后转到http：// localhost /并浏览向导。默认情况下，此容器使用SQLite进行数据存储，但向导应允许连接到现有数据库。另外，6.0，7.0或8.0的标签是可用的。

对于MySQL数据库，您可以链接数据库容器，例如--link my-mysql:mysql，然后mysql在安装时用作数据库主机。

## 资源链接

- https://owncloud.org/
- https://doc.owncloud.org/
