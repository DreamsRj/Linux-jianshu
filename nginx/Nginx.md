# Nginx

## 安装[Centos 7]

编辑源

```shell
vim /etc/yum.repos.d/nginx.repo
```

录入以下内容

```shell
[nginx]
name=nginx repo
baseurl=http://nginx.org/packages/mainline/centos/7/$basearch/
gpgcheck=0
enabled=1
```

安装

```shell
yum install nginx
```



将 Nginx 加入开机启动和 systemctl命令控制

```shell
sudo systemctl enable nginx
```



## 开启80/443 端口

```shell
sudo firewall-cmd --permanent --zone=public --add-service=http
sudo firewall-cmd --permanent --zone=public --add-service=https
sudo firewall-cmd --reload
```





## 配置

- Config dir – **/etc/nginx/**
- Master/Global config file – **/etc/nginx/nginx.conf**
- Port 80 http config file – **/etc/nginx/conf.d/default**
- TCP ports opened by Nginx – **80 (HTTP), 443 (HTTPS)**
- Document root directory – **/usr/share/nginx/html**



## 将AdminLTE作为测试服务

将 AdminLTE 目录下的内容放到 /usr/share/nginx/html 下, 重启nginx