---
layout: post
title: Shadowsocks scripts
tags:
  - Shadowsocks
  - ss
---
```bash
wget --no-check-certificate -O shadowsocks-all.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-all.sh
chmod +x shadowsocks-all.sh
./shadowsocks-all.sh 2>&1 | tee shadowsocks-all.log
```
Source: [Teddysun's Blog](https://teddysun.com/486.html)
```bash
iptables -A INPUT -p tcp --dport PORTNUMBER -j ACCEPT
iptables -F 
netstat -apn | grep PORTNUMBER
```
Source: [Michany's Blog](https://blog.michany.com/2020/01/13/Ubuntu-Shadowsocks/)


