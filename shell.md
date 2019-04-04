# shell

### tar
```shell
# pack
tar -zcvf api_view.tar.gz  --exclude=node_modules --exclude=.git --exclude=.idea ./
# unpack
tar -xzvf ***.tar.gz
```

### zip
```shell
zip -r layout_view.zip ./*
```

### fs
```shell
du -h --max-depth=1 /opt/files/
```

### tail
```shell
tail -f api_out.log
```
- 从3000行开始，显示1000行，即显示3000~3999行
```shell
cat filename | tail -n +3000 | head -n 1000
```
- 显示1000行到3000行
```shell
cat filename | head -n 3000 | tail -n +1000
```
 - 根据关键字查看日志
```shell
cat filename | grep "keyword"
cat api_out.log | grep "train"
grep -I " keyword" filename
grep -I "train" api_out.log
```
