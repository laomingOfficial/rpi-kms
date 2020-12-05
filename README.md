# 樹莓派架設KMS服務器

只供學習使用，請支持正版Windows和Office！

安装步骤指令(Command):
1) wget https://github.com/kkkgo/vlmcsd/releases/download/1113/Linux-arm-1113.zip
2) unzip Linux-arm-1113.zip -d ./vlmcsd
3) cd vlmcsd
4) sudo cp ./vlmcsd-armv7el-glibc /usr/bin/vlmcsd
5) sudo chmod +x /usr/bin/vlmcsd
6) sudo wget -O /etc/systemd/system/vlmcsd.service https://raw.githubusercontent.com/laomingOfficial/rpi-kms/master/vlmcsd.service

Service服务指令:  
```
重载所有修改过的配置文件  
sudo systemctl daemon-reload  

启动服务  
sudo systemctl start vlmcsd  

将服务设置为开机启动  
sudo systemctl enable vlmcsd  

停止运行服务  
sudo systemctl stop vlmcsd  

将服务设置为禁止开机启动  
sudo systemctl disable vlmcsd  

检测服务状态  
sudo systemctl status vlmcsd  
```
