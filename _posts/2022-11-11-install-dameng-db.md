---
title: Install dameng database
---

# Install by docker
```

docker run -d -p 5236:5236 --restart=always --name dm8_01 --privileged=true -e CASE_SENSITIVE=N -e UNICODE_FLAG=1 -e LENGTH_IN_CHAR=Y -e PAGE_SIZE=8 -e LD_LIBRARY_PATH=/opt/dmdbms/bin -e INSTANCE_NAME=dm8_01 -v /data/dm8_01:/opt/dmdbms/data dm8_single:v8.1.2.128_ent_x86_64_ctm_pack4


```
