---
title: Port Forwarding Cheatsheet
published: true
---

**YEET**

Good Material:
https://help.ubuntu.com/community/SSH/OpenSSH/PortForwarding


LOCAL PORT FORWARDING
ssh -L


ssh user@host -L 5555:127.0.0.1:5555 -p 22


REMOTE PORT FORWARDING
ssh -R 


DYNAMIC PORT FORWARDING
< turns ssh into a socks proxy >
ssh -C -D 1080 laptop

→ -C for Compression, speeds up HTTP, slows down downloading binaries
→ -D for Dynamic
→ 1080 for default SOCKS port, some programs will only work with it (leave default)
