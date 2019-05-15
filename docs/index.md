# caddy配置文档 Caddyfile

## 简介
Caddy 是一款Go语言编写的 Web server ，官网：[https://caddyserver.com](https://note.youdao.com/) 

简单说，caddy的优点就是首页所宣传的：实现任何网站全自动化的HTTPS，网站SSL证书不用你管，全自动搞定自动续期更新。这对于即使使用了acme.sh之类的自动脚本，还需要额外设置Cron，并且还可能失效的，方便太太多了。
```
EVERY site on HTTPS    
Caddy is the HTTP/2 web server with automatic HTTPS.
```
另外就是Caddy的配置文件非常简化、易读，可以看一眼就能明白，看两次你就能自己写。而默认的配置文件就是`Caddyfile` 

## 安装
[https://caddyserver.com/download](https://note.youdao.com/)  选择系统、插件、勾选个人授权（免费），例如 `curl https://getcaddy.com | bash -s personal`
默认安装在 /usr/local/bin 目录，因此建议将配置文件 Caddyfile （没有扩展名，C为大写）放在同样的目录下，方便测试和使用。
caddy -conf /u
