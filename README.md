# docker-lnmp



本机的环境是在linux下的，暂未尝试在win下兼容。建议在linux下使用此环境。如果在win下，还是建议一键的集成环境，如[phpstudy](http://phpstudy.php.cn/download.html?yyue=a21bo.50862.201879)和[xampp](https://www.apachefriends.org/zh_cn/index.html)。

# 搭建教程

### 安装docker和docker-compose和git

运行docker -v   有  `Docker version 17.09.1-ce, build 19e2cf6`类似这样的返回

运行docker-compose -v 有 `docker-compose version 1.17.1, build 6d101fb`类似这样的返回即安装成功。(注意：docker-compose 版本如果较老可能会导致构建容器失败，请将docker-compose更新到最新版)

### 使用`git`下载完整代码：

```
$ git clone https://github.com/jinchaojian/docker-lnmp.git
```

### 用`docker-compose`命令启动容器

在项目根目录下运行`docker-compose up`命令构建容器。

```
$ docker-compose up
```

##### docker-compose常用命令

| docker-compose up    | 根据docker-compose.yml构建容器 |
| -------------------- | ------------------------------ |
| docker-compose start | 启动容器，无需重新构建         |
| docker-compose stop  | 停止容器                       |
| docker-compose ps    | 查看有哪些服务                 |

### 然后在浏览器中访问`localhost：8989`，就可以访问到项目的web目录：

web目录在：`./app/src` 目录下。



