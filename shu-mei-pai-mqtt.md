# 树莓派MQTT客户端安装

## 1.下载

```
CD MQTT 
git init 
git pull https://github.com/eclipse/mosquitto.git
```

## 2. 安装

编译前需安装必须的相关包

```
sudo apt-get update
sudo apt-get install libssl-dev uuid-dev xsltproc docbook-xsl libc-ares-dev libc-ares2
```

编译 安装

```
make
sudo make install
```

编译过程找不到ares.h

修改config.mk中的WITH\_SRV:=yes，改为WITH\_SRV:=no

其他问题没有碰到，如果有自行搜索解决。

