tool for operate qcloud load balancer

install

```
sudo apt-get install jq
git clone https://github.com/ljsdk/qlb.git
cd qlb/
sudo ./install 
sudo vi /etc/qlb.conf
```

Usage
```
qlb [OPTION] [NAME]
--conf=FILE
        use FILE as config file, default config file is /etc/qlb.conf
--create=NAME
        create new load balancer with name NAME
--delete=NAME
        delete load balancer with name NAME
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
