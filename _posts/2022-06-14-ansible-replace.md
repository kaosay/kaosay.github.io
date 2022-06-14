---
title: ansible replace model
---

# ansible replace
```
---
- name: replace 16.241
  hosts: tmp
  
  tasks:
  - name: replace hc
    become: yes
    become_user: root
    replace:
      path: /etc/ssh/sshd_config
      regexp: 'a'
      replace: 'b'
      backup: yes


```
