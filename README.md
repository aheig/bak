# Download & Install  Tcping for macOS
```
wget https://github.com/paradiseduo/tcping/releases/download/3.2/tcping.zip
unzip tcping.zip
chmod +x tcping
mv tcping /usr/local/bin/
sudo xattr -rd com.apple.quarantine /usr/local/bin/tcping
```

# Download & Install Web
```
cd /usr/share/nginx/html
wget https://raw.githubusercontent.com/aheig/bak/main/web3.zip
unzip web*.zip
systemctl restart nginx
```

# Download & Install Docker
```
wget https://raw.githubusercontent.com/aheig/bak/main/docker.sh && bash ./docker.sh
```
# Nssm 是一个创建服务命令

示例：

创建服务  `` nssm install [服务名]   ``

启动服务  ``nssm start [服务名]   ``

删除服务  ``nssm remove [服务名]   ``

