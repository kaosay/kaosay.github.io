---
title: disk extend
---

# extend
```
#LV动态增加磁盘大小:



pvcreate /dev/sdk

vgextend VolGroup00 /dev/sdk   #将pv加入到VG(VolGroup00)中

lvextend -l +100%FREE  /dev/VolGroup00/LVdata1   #将VG(VolGroup00)中所有的余量加入到LV(LVdata1)中

xfs_growfs  /dev/VolGroup00/LVdata1   #(加入后动态加入要需要使用xfs_growfs动态收缩磁盘)

```
