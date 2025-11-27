# minio

minio-console.8and1.cn

#### 数据迁移

install mc
```bash
#新服务器执行
wget https://dl.min.io/client/mc/release/linux-amd64/mc
chmod +x mc
sudo mv mc /usr/local/bin/mc

```


```bash
#旧服务器执行
mc alias set local http://127.0.0.1:9000 root *******
mc alias set destination http://223.109.200.118:9000 root *******

#新服务器执行
mc mb local/static

#旧服务器执行
mc mirror local/static destination/static

```


