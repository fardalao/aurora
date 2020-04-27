Aurora is a v2ray server that only supports the v2board panel.

This project is a paid project to make us serve you better.

Buy it telegram @v2aurora

Last update at: **2020.04.27 v1.2.4**

## Use

Debian or centos please run
```
curl -fsSL https://github.com/tokumeikoi/aurora/raw/master/install.sh | bash -s API TOKEN NODEID LOCALPORT LICENSE SYNCINTERVAL
```

docker please run
```
Docker run -d --name=aurora \
-p 连接端口:连接端口 \
-p 连接端口:连接端口/udp \
-e API=API \
-e TOKEN=TOKEN \
-e NODE=NODEID \
-e LICENSE=LICENSE \
-e SYNCINTERVAL=60 \
tokumeikoi/aurora

# 连接端口同V2board连接端口
```

|Params|Description|Require|
|:---|:---|:---|
|API|https://xxxx.com|Yes|
|TOKEN|通讯密钥|Yes|
|NODEID|节点ID|Yes|
|LICENSE|授权码|Yes|
|LOCALPORT|本地端口，用于与V2ray通讯使用，如果本地有部署多个请不要冲突，也不要与连接端口或服务端口冲突|Yes|
|SYNCINTERVAL|数据提交频率，默认60秒/次|No|

## Old version  
https://github.com/tokumeikoi/aurora/releases

## Build
```
https://github.com/tokumeikoi/aurora.git
docker build ./aurora
```
