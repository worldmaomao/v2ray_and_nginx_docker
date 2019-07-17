# v2ray_and_nginx_docker




## 原理：
1.v2ray + websocket方式

2.在v2ray前面，使用nginx做反向代理，

## 需要修改的地方：
1.修改端口。只要修改docker-compose.yml文件里配置（"23143:80"），默认端口是23143。
修改23143为其他端口，:（冒号）后面的80不要修改。

2.修改v2ray的uuid。修改v2ray/server.json文件里的配置（inbounds -> settings -> clients -> id）。
uuid的生成方式：
a)访问http://www.uuid.online/ 
b)cat /proc/sys/kernel/random/uuid


## 启动方式：
1.安装好docker，docker-compose

2.执行命令: docker-compose up -d










