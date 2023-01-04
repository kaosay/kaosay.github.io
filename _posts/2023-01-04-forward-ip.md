---
title: Linux forward ip
---

# How to forward ip
```

firewall-cmd --get-active-zones

firewall-cmd --get-default-zone

firewall-cmd --set-default-zone=public

firewall-cmd --query-masquerade

firewall-cmd --add-masquerade --permanent

firewall-cmd --add-forward-port=port=9071:proto=tcp:toport=9071:toaddr=10.232.141.21 --permanent

firewall-cmd --reload

firewall-cmd --list-all

```
