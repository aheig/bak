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
wget https://raw.githubusercontent.com/aheig/bak/main/web.zip
unzip web.zip
systemctl restart nginx
```
