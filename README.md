# 快速 setup node server

初始化目录: `npm init`

安装 http server: `npm install http-server`

开启 http server: `http-server [path] [options]`

Server 端添加 `crontab`:

```bash
crontab -e
*/1 * * * * /bin/sh -c 'cd /var/www/event-output && git fetch --all && git reset --hard origin/master'
```
