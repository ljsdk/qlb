##通过shell命令操作腾讯云负载均衡
* 支持创建、绑定端口、注册后端等功能

##对原有http api做了一些简化和限制：
* 负载均衡前后端端口必须相等
* 只支持内网无日租、tcp协议的负载均衡操作

##install

```
sudo apt-get install jq curl
git clone https://github.com/ljsdk/qlb.git
cd qlb/
sudo ./install 
sudo vi /etc/qlb.conf
```

##Usage
```
qlb [OPTION] [NAME]
--conf=FILE
        use FILE as config file, default config file is /etc/qlb.conf
--create
        create new load balancer
--delete
        delete load balancer
--listen=PORT
        load balancer listen to PORT. (load balancer port and backend port are same)
--unlisten=PORT
        unlisten PORT
--regist=INSTANCE
        regist INSTANCE to load balancer
--deregist=INSTANCE
        deregist INSTANCE from load balancer
--regist-local
        regist local to load balancer
--deregist-local
        deregist local from load balancer
```
