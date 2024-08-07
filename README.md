# Serv00搭建各种服务

## 相关网站

Serv00搭建各种服务：https://saika.us.kg/2024/01/27/serv00_logs

Serv00：https://www.serv00.com

FreeBSD cloudflared：https://cloudflared.bowring.uk

站点监测：https://uptimerobot.com

## 常见问题

### Serv00会不定期重启，可以使用以下命令重新加载保存的应用列表：

```
pm2 resurrect
```

### 由于 S8 服务器禁止访问 cloudflared.bowring.uk，可以使用以下命令来下载 Cloudflared：

```
bash <(curl -s https://raw.githubusercontent.com/jinnan11/serv00-api/main/cf-f.sh)
```

### pm2常用指令

pm2 list # 显示所有进程状态

pm2 stop all # 停止所有进程

pm2 restart all # 重启所有进程

pm2 save # 保存当前应用列表

pm2 resurrect # 重新加载保存的应用列表

pm2 delete all # 删除某个应用程序
