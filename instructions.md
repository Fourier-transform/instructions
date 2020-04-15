```
java -jar -Djava.rmi.server.hostname=192.168.21.135 -Dcom.sun.management.jmxremote.port=8081 -Dcom.sun.management.jmxremote.rmi.port=8081 -Dcom.sun.management.jmxrete.ssl=false -Dcom.sun.managemenjmxremote.authenticate=false  aaa-1.1.0.jar  远程debug
```
```
scp /root/apache-tomcat-8.5.30/webapps/web-server.war root@remoteIp:/root/apache-tomcat-8.5.30/webapps/  
scp -r /root/project/ root@remoteIp:/root/  本地到远程 -r 递归文件夹
scp root@remoteip:/home/xxxx.jar  D:/  win执行，远程到本地
```
```
tcpdump -i ens33 src host 192.168.21.1 #抓包 指定源ip
ulimit -HSn 102400
```
```
git remote add origin  https://github.com/user/repo.git  #添加/新建 远程仓库
git add .
git commit -m 'First commit'
git push -u origin master
```
```
#go module proxy
https://goproxy.cn
https://goproxy.io
```
```
netsh wlan show profiles #显示本机所有wifi
netsh wlan show profile WiFi-name key=clear #显示特定wifi信息
```
