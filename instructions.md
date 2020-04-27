```
远程debug
java -jar -Djava.rmi.server.hostname=192.168.21.135 -Dcom.sun.management.jmxremote.port=8081 -Dcom.sun.management.jmxremote.rmi.port=8081 -Dcom.sun.management.jmxrete.ssl=false -Dcom.sun.managemenjmxremote.authenticate=false  aaa-1.1.0.jar  
```
```
拷贝文件
scp /root/apache-tomcat-8.5.30/webapps/web-server.war root@remoteIp:/root/apache-tomcat-8.5.30/webapps/  
scp -r /root/project/ root@remoteIp:/root/  本地到远程 -r 递归文件夹
scp root@remoteip:/home/xxxx.jar  D:/  win执行，远程到本地
```
```
tcpdump -i ens33 src host 192.168.21.1 #抓包 指定源ip
ulimit -HSn 102400
```
```
#git 添加/新建 远程仓库 
git remote add origin  https://github.com/user/repo.git  
git add .
git commit -m 'First commit'
git push -u origin master
```
```
#go module 代理
https://goproxy.cn
https://goproxy.io
```
```
WIFI信息 windows
netsh wlan show profiles #显示本机所有wifi
netsh wlan show profile WiFi-name key=clear #显示特定wifi信息
```
```
防火墙
firewall-cmd --permanent --zone=public --add-port=8080/tcp 防火墙开放8080端口
firewall-cmd --permanent --zone=public --remove-port=8080/tcp 删除端口
firewall-cmd --zone=public --add-port=8080-8090/tcp --permanent 添加地址段
firewall-cmd --reload 加载后修改才生效
firewall-cmd --zone=public --list-ports 查看开放端口
firewall-cmd --zone=public --list-services 查看开放服务
```
