# 树莓派MQTT客户端安装

## 1.下载

```
CD MQTT 
git init 
git pull https://github.com/eclipse/mosquitto.git
```

## 2. 安装

\# 编译 安装

```
make
sudo make install
```

1. 编译找不到openssl/ssl.h   ，需安装openssl

```
sudo apt-get update
sudo apt-get install libssl-dev
```

1. 编译过程找不到ares.h
   修改config.mk中的WITH\_SRV:=yes，改为WITH\_SRV:=no



