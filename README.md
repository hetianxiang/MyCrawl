## 项目描述
```
1.express+request+cheerio+async+mongodb ；
2.抓取'http://top.baidu.com/buzz?b=26'网站中电影标题；
3.渲染到新页面；
4.阿里云上线

```

## 初始化项目
```
npm init -y
```

## 安装依赖的模块
```
npm install request cheerio async cron debug mongoose express ejs iconv-lite -S
```

## 连接服务器
### 连接服务器
如果需要是否yes,yes,如果需要输入密码 Zfpx2017
```
ssh root@ip
ssh root@120.27.250.23
```

### 更新操作系统
```
apt-get update
```

### 安装 npm
```
apt-get install npm
```

### 安装node的版本管理器
```
npm install n -g
```

### 安装 node
```
n 7.5
```

### 安装 mongodb
```
apt-get install mongodb
```

### 安装git
```
apt-get install git
```

### 下载并安装项目
```
git clone https://github.com/zhufengnodejs/201703crawl.git
cd 201703crawl
npm install

cd tasks
node main.js
ctrl+c退出

cd ..
node server.js
```
然后就可以通过浏览器(主机加端口号)访问我们的服务器


### 安装pm2
因为我们希望我们的服务在后台运行
```
npm install pm2 -g
pm2 start server.js --name 'crawl'
pm2 list	查看所有应用
pm2 restart crawl	重启应用
pm2 stop crawl	停止应用
pm2 delete crawl	删除应用
```

## 安装nginx
Nginx是一个高性能的HTTP和反向代理服务器
```
apt-get install nginx
```

## nginx命令
```
启动nginx nginx -c /etc/nginx/nginx.conf
关闭 nginx nginx -s stop
重读配置文件nginx -s reload kill -HUP nginx
常用命令service nginx {start|stop|status|restart|reload|configtest|}

```