---
title: monitor tcp port on Zabbix
---

# Item
```
Key: net.tcp.port[172.0.0.1,80]

Update interval: 20s

```


#Trigger
```
Expression: {gov_port:net.tcp.port[172.0.0.1,80].sum(#2)}=0

```
