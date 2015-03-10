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

qlb 
qlb --create lb1
qlb --delete lb1
qlb --listen 8000 lb1
qlb --unlisten 8000 lb1
qlb --regist vm1 lb1
qlb --deregist vm1 lb1
qlb --regist-local lb1
qlb --deregist-local lb1
qlb --conf /etc/qlb.conf 

