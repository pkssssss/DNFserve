#### 集成环境:

curl -O https://pkssssss.github.io/dnfserve/lamp;chmod +x lamp;./lamp

#### 纯端文件:

curl -O https://pkssssss.github.io/dnfserve/dnf;chmod +x dnf;./dnf

#### 集成环境+纯端文件:

curl -O https://pkssssss.github.io/dnfserve/lamp+dnf;chmod +x lamp+dnf;./lamp+dnf

------

```shell
启动命令：./run                     关闭命令：./stop

PHP默认端口：80                     PHP目录：/opt/lampp/htdocs          

数据库目录：/opt/lampp/var/mysql

端口配置文件：/opt/lampp/etc/httpd.conf
```

------

#### 重启PHP

```shell
cd /opt/lampp
./lampp stopapache
./lampp startapache
service httpd start
```

#### 重启Mysql

```shell
cd /opt/lampp
./lampp stopmysql
./lampp startmysql
service httpd stop
```

------

#### 登录器组件

> yum install -y php-gd* php php-mysql openssl httpd php-mysql

```shell
# 文件名：CentOS-Base5.repo
# CentOS-Base5.repo
#
#
[share]
name=mysharesource
baseurl=http://zidc.oss-cn-beijing.aliyuncs.com/Repo/
gpgcheck=0
```
