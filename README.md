# ComposeHub
ComposeHub 是一个用来分享有趣、实用的 Docker 容器的 Docker Compose 的项目。你可以在这里直接下载或复制容器的 Docker Compose，然后进行部署。Docker Compose 中需要进行修改的部分都有说明，抄作业比较方便。

## 需要修改的部分
- **自定义目录**：通常是用来设置容器的应用/用户数据的存储位置的，按需要进行设置。
- **PUID/PGID**：用户 ID 和组 ID，用来设置容器以什么身份/权限运行。MacOS、Linux 和 NAS 用户可以在终端或 SSH 中通过命令 `id -u 用户名` 和 `id -g 用户名` 查询自己的 PUID 和 PGID，Windows 用户可以直接设置为 `1000`（`0` 代表 root 用户，`1000` 或其他值代表非 root 用户，若没有特殊要求一般使用自己的 ID）。
- **端口**：`ports` 这个部分是用来设置容器端口的，例如 `5244:5244`，左侧表示宿主机上的端口号，右侧表示 Docker 容器内部的端口号，一般情况下无需改动，若端口号存在冲突或有其他需求，可以修改左侧的端口号，例如 `5044:5244`，这样你在宿主机上访问 `5044` 端口时，你的请求会被转发到 Docker 容器的 `5244` 端口，从而到达你的应用。
- **其他配置**：若还存在其他需要自定义的配置选项，请根据说明按需要进行设置。

## 容器列表
1. [AList-STRM](https://github.com/tefuirZ/alist-strm)：一个用于为 AList 生成 STRM 文件的工具，可用于网盘文件 302 直链或免挂载入库，有 WebUI。
2. [AList](https://alist.nn.ci/zh/)：一个支持多种存储的文件列表程序，提供文件预览和下载功能，支持通过 WebDAV 访问网盘。
3. [Aliyundrive Subscribe](https://github.com/adminpass/aliyundrive-subscribe)：阿里云盘订阅，自动订阅、转存、重命名、下载、签到、搜索和资源管理工具。
4. [AutoFilm](https://github.com/Akimio521/AutoFilm)：一个用于为 AList 生成 STRM 文件的工具，可用于网盘文件 302 直链或免挂载入库。
5. [Chinese Localization for Plex](https://github.com/x1ao4/chinese-localization-for-plex)：Plex 拼音排序、拼音搜索及标签汉化工具。
6. Clear 115 Share Dir：定时自动清空 115 网盘我的接收或回收站的工具，支持自定义执行周期。
7. [CloudDrive](https://www.clouddrive2.com/index.html)：一个强大的多云盘管理工具，为用户提供包含云盘本地挂载的一站式多云盘解决方案。
8. [DeepL API](https://hub.docker.com/r/zu1k/deepl)：通过逆向 DeepL 客户端使用的协议，实现的免费 DeepL API。
9. [Docker Copilot](https://github.com/onlyLTY/dockerCopilot)：Docker 助手，支持一键更新容器、删除未使用镜像、备份容器设置、恢复容器设置等功能。
10. [Dockge](https://github.com/louislam/dockge)：一个 Docker Compose 堆栈管理工具，支持集中管理 Docker Compose 和监视应用等功能。
11. [Dufs](https://github.com/sigoden/dufs)：一个开源文件服务器，支持文件管理、搜索和访问控制等功能，可为本地存储提供 WebDAV 服务。
12. [Edition Manager for Plex](https://github.com/x1ao4/edition-manager-for-plex)：Plex 电影版本（Edition）管理工具。
13. [HandBrake](https://github.com/jlesage/docker-handbrake)：一款开源、跨平台的视频转换/转码工具，内置了多种预设方案，支持批量转换。
14. [IPTV Checker](https://github.com/zhimin-dev/iptv-checker)：M3U 直播源有效性检测工具，支持批量管理源、删除无效源，并提供了一些直播源。
15. [Lucky](https://lucky666.cn/)：软硬路由公网神器，支持端口转发、反向代理、动态域名、网络唤醒、内网穿透、免费自动证书等功能。
16. [MDC-NG](https://github.com/mdc-ng/mdc-ng)：视频刮削工具，支持刮削元数据、整理文件等功能，支持下载、处理图片，可生成 NFO 文件。
17. [MKVToolNix](https://github.com/jlesage/docker-mkvtoolnix)：一款用于创建、编辑、分割、合并和检查 MKV 媒体文件的工具，可用于压缩或 Remux 媒体文件。
18. [Music Tag Web](https://github.com/xhongc/music-tag-web)：音乐标签编辑工具，支持从国内外音乐平台刮削元数据并写入标签，支持批量处理。
19. [Nginx Proxy Manager](https://nginxproxymanager.com/)：一个简单易用的 Nginx 代理主机管理工具，支持反向代理、免费自动证书等功能。
20. [Pixman](https://hub.docker.com/r/pixman/pixman)：通过自建服务器，使用自己的 IP 地址或域名访问由作者维护的 IPTV 直播源。
21. [Plex Auto Languages](https://github.com/RemiRigal/Plex-Auto-Languages)：Plex 电视节目音频、字幕自动选择工具，可自动将单集的选择应用到全剧。
22. [Plex Auto Skip](https://github.com/mdhiggins/PlexAutoSkip)：通过远程控制实现局域网内连接 Plex 服务器的设备在播放时自动跳过片头尾和自动连续播放。
23. [Plex Trakt Sync](https://github.com/Taxel/PlexTraktSync)：一个用于同步 Plex 与 Trakt 的观看记录、评分和收藏等信息的工具，支持实时同步。
24. [RSSHub](https://docs.rsshub.app/)：一个开源、简单易用、易于扩展的 RSS 生成器，可以为任何内容生成 RSS 订阅源。
25. [Stream Master](https://github.com/SenexCrenshaw/StreamMaster)：一个 M3U 代理服务平台，支持导入、管理 M3U 和 EPG，提供串流分析和统计工具。
26. [Threadfin](https://github.com/Threadfin/Threadfin)：一个基于 xTeVe 构建的专为 Plex DVR 和 Emby/Jellyfin Live TV 设计的 M3U 代理服务器。
27. [Uptime Kuma](https://github.com/louislam/uptime-kuma)：一个自托管的服务器监控工具，支持多种监控方式和通知服务。
28. [xTeVe](https://github.com/xteve-project/xTeVe)：一个 M3U 代理服务器，专为 Plex DVR 和 Emby Live TV 设计，支持合并、管理外部 M3U 和 XMLTV。
29. [YunPlex](https://github.com/awillheartwu/yunplex)：一个用来同步 Plex 音乐资料库和网易云音乐歌单的工具。

## 赞赏
如果你觉得这个项目对你有用，可以请我喝杯咖啡。如果你喜欢这个项目，可以给我一个⭐️。谢谢你的支持！

<img width="399" alt="赞赏" src="https://github.com/x1ao4/ComposeHub/assets/112841659/9f1b8962-a4e0-498e-8e8a-661cdbc8d2b3">
