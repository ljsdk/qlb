##通过shell命令操作腾讯云负载均衡

##example
```
#取消本机和负载均衡lb1之间的关联
qlb --deregist-local lb1

#重新部署或者重启服务

#关联本机和负载均衡lb1
qlb --regist-local lb1
```

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
