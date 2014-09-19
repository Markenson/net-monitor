net-monitor
===========

Simple java network port monitor

How build it?
=============

After clone it, install maven and type the following command:

```
mvn clean install
```

How use it?
===========

type:
```
java -jar target/net-monitor-1.0-SNAPSHOT.jar [src_ip] [dest_ip] [port]

src_ip - IP of source ethernet board
dest_ip -IP of destiny ethernet board
port - port to monitor
```
example:
```
java -jar target/net-monitor-1.0-SNAPSHOT.jar 192.168.1.8 173.194.42.159 80
```

output if can connect:
```
Thu Sep 18 23:05:16 BRT 2014 173.194.42.159:80 [CONNECTED]
Thu Sep 18 23:05:17 BRT 2014 173.194.42.159:80 [CONNECTED]
Thu Sep 18 23:05:18 BRT 2014 173.194.42.159:80 [CONNECTED]
Thu Sep 18 23:05:19 BRT 2014 173.194.42.159:80 [CONNECTED]
Thu Sep 18 23:05:20 BRT 2014 173.194.42.159:80 [CONNECTED]
```
output if can't connect:
```
Thu Sep 18 23:05:21 BRT 2014 173.194.42.159:80 [DISCONNECTED]
Thu Sep 18 23:05:22 BRT 2014 173.194.42.159:80 [DISCONNECTED]
Thu Sep 18 23:05:23 BRT 2014 173.194.42.159:80 [DISCONNECTED]
Thu Sep 18 23:05:24 BRT 2014 173.194.42.159:80 [DISCONNECTED]
Thu Sep 18 23:05:25 BRT 2014 173.194.42.159:80 [DISCONNECTED]
```
