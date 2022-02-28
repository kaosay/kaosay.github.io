---
title: nginx configure
---

# Translate 80 to 443
```

server {
    listen 80;
    listen [::]:80;
    server_name kaosay.shop;
    return 301 https://$server_name:42729$request_uri;
}

```
