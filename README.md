感恩原作者rico辛苦付出，本人仅做备份和后续维护，caddy镜像更新支持tls1.3。

使用教程请看wiki。

既然破解版都泛滥了我也放出来吧，此版本有审计和数据库对接。

bbr加速：
```
wget -N --no-check-certificate "https://raw.githubusercontent.com/wanglu58/Linux-NetSpeed/master/tcp.sh"
chmod +x tcp.sh
./tcp.sh
```

关闭防火墙：
```
systemctl stop firewalld.service
systemctl disable firewalld.service
```

安装docker：
```
docker version > /dev/null || curl -fsSL get.docker.com | bash
service docker restart
systemctl enable docker
```

运行脚本：
```
mkdir v2ray-agent
cd v2ray-agent
curl https://raw.githubusercontent.com/wanglu58/SSPanel-UIM-v2plugin/master/install.sh -o install.sh
chmod +x install.sh
./install.sh
```

重新运行脚本（不要重复输入上面的命令）：
```
cd v2ray-agent
./install.sh
```

免责声明：

本程序仅供学习了解，请于下载后 24 小时内删除，不得用作任何商业用途，文字、数据及图片均有所属版权，如转载须注明来源。

使用本程序必循遵守部署服务器所在地、所在国家和用户所在国家的法律法规，程序作者不对使用者任何不当行为负责。
