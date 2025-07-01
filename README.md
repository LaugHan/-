# -
记录怎么在Linux(Ubuntu)上面配置代理

首先是下载clash这个文件，然后解压
```
wget https://github.com/MetaCubeX/mihomo/releases/download/v1.19.11/mihomo-linux-amd64-v1.19.11.gz -O clash.meta.gz
gzip clash.meta.gz
chmod +x clash.meta
mv clash.meta clash
```


然后是得到clash的配置文件config.yaml
```
wget -O config.yaml "xxxxxxx为clash提供的网址"
# 就是clash 订阅的网址
```

然后参考 https://blog.51cto.com/u_15531854/8921380 配置mmdb文件，最后反复执行（可能会现实mmdb文件invalid，但是多运行几次就可以了）
```
./clash -f config.yaml
```

