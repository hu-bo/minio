# minio

minio-console.8and1.cn

#### 数据迁移

install mc
```bash
wget https://dl.min.io/client/mc/release/linux-amd64/mc
chmod +x mc
sudo mv mc /usr/local/bin/mc

```


```bash
mc alias set local http://127.0.0.1:9000 root *******
mc alias set destination http://106.75.237.2487:9000 root *******
mc mirror source/static destination/static
```