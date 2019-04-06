java -jar -Djava.rmi.server.hostname=192.168.21.135 -Dcom.sun.management.jmxremote.port=8081 -Dcom.sun.management.jmxremote.rmi.port=8081 -Dcom.sun.management.jmxrete.ssl=false -Dcom.sun.managemenjmxremote.authenticate=false  aaa-1.1.0.jar

tcpdump -i ens33 src host 192.168.21.1

ulimit -HSn 102400