# What is it?
这是一款可自动抓取远程 m3u 列表的工具，它能够对列表中的频道进行分析，接着测试频道的可用性与延迟情况，最终解析出频道的视频和音频流信息存储到本地数据库里。

# Features
- 自动抓取远程 m3u 列表。
- 自动将频道存储至本地数据库。
- 定时检测频道的可用性以及连接耗时。
- 定时解析频道的视频音频流信息。
- 支持在线管理所有频道。
- 提供 m3u 频道列表地址。

# M3U List
可以在直播软件里通过添加自定义直播源的方式添加这些地址来收看直播频道。

### Subscription 1 (Auto Update)
```
所有频道：
https://raw.githubusercontent.com/big-mouth-cn/m3u8-checker/main/iptv.m3u

仅当前可用的频道：
https://raw.githubusercontent.com/big-mouth-cn/m3u8-checker/main/iptv-ok.m3u
```

### Subscription 2
```
http://127.0.0.1:8080/m3u/list?justOk=1&withoutRepeat=1
```

**参数说明**
  - `justOk`：值 `1` 只显示可用频道。
  - `withoutRepeat`：值 `1` 过滤重复频道，保留视频分辨率最高的频道。重复的定义是：频道名称。

# Manage Channel
可以在浏览器里通过访问 `http://127.0.0.1:8080/mgr.html` 来管理频道。

![显示所有频道](docs%2FiShot_2024-11-20_17.54.03.png)

![编辑频道](docs%2FiShot_2024-11-20_17.58.57.png)

**本工具仅供学习交流使用。**