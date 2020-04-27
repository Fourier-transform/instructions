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
#抓包 指定源ip
tcpdump -i ens33 src host 192.168.21.1 
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
systemctl status firewalld 查看状态 ,参systemctl
firewall-cmd --permanent --zone=public --add-port=8080/tcp 防火墙开放8080端口
firewall-cmd --permanent --zone=public --remove-port=8080/tcp 删除端口
firewall-cmd --zone=public --add-port=8080-8090/tcp --permanent 添加地址段
firewall-cmd --reload 重启加载后修改才生效
firewall-cmd --zone=public --list-ports 查看开放端口
firewall-cmd --zone=public --list-services 查看开放服务
```
```
systemctl指令
systemctl list-units            ##列出当前系统服务的状态
systemctl list-unit-files       ##列出服务的开机状态
systemctl status sshd           ##查看指定服务的状态
systemctl stop sshd             ##关闭指定服务
systemctl start sshd            ##开启指定服务
systemctl restart sshd          ##从新启动服务
systemctl enable sshd           ##设定指定服务开机开启
systemctl disable sshd          ##设定指定服务开机关闭
systemctl reload sshd           ##使指定服务从新加载配置
systemctl list-dependencies sshd    ##查看指定服务的倚赖关系
systemctl mask  sshd            ##冻结指定服务
systemctl unmask sshd           ##启用服务
```
