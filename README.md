# Aini Player

一款轻量的 Android 影视播放器，支持导入自定义 **Python 源**，本地代理转发、海报缓存、片头跳过与播放嗅探一应俱全。

> 本仓库**只发布安装包，不包含源码**。

![version](https://img.shields.io/badge/version-1.59.25-blue)
![android](https://img.shields.io/badge/Android-7.0%2B-green)
![target](https://img.shields.io/badge/targetSdk-36-lightgrey)

---

## 下载

前往 [Releases](../../releases/latest) 页面下载最新版 `AiniPlayer-x.x.x.apk` 安装即可。

国内访问较慢时，可在原下载地址前加上加速前缀：

```
https://ghproxy.net/https://github.com/wangzide601/Aini-Player/releases/download/v1.59.25/AiniPlayer-1.59.25.apk
```

## 功能

- **自定义源**：支持标准 Python 源（`class Spider`），从首页「打开影视源」或文件管理器直接打开 `.py` 文件
- **本地代理**：内置本地 HTTP 代理服务，自动为图片/播放地址补 Referer，解决图床与 CDN 防盗链
- **播放引擎**：基于 Media3 / ExoPlayer，支持 HLS、软硬解切换、倍速、记忆播放进度
- **本地播放**：支持本地常见视频格式（MP4 / MKV / AVI / MOV / FLV / TS / WebM 等）直接播放
- **播放嗅探**：自动从网页中嗅探 m3u8 / mp4 直链
- **海报缓存**：内存 + 磁盘二级缓存，滚动不重复拉图
- **字幕与歌词**：支持外挂字幕、LRC 歌词解析
- **跳过片头**：按源记忆片头时长，下次自动跳过
- **主题皮肤**：多套配色与壁纸

## 演示视频

https://github.com/user-attachments/assets/13a2bbaf-423b-4aee-8954-7d124a3d2e55

https://github.com/user-attachments/assets/b0383371-8c62-494a-b1e4-53944e7fdd43

## 系统要求

| 项目 | 要求 |
|---|---|
| 系统版本 | Android 7.0（API 24）及以上，建议 Android 10+ |
| 存储 | 约 60 MB 可用空间 |
| 网络 | 需联网；播放依赖所导入的源 |

## 安装

1. 下载 APK；
2. 首次安装需在系统设置中允许「安装未知来源应用」；
3. 安装完成后打开，在首页点击 **「打开影视源」** 选择 `.py` 源文件；也可以从文件管理器直接点 `.py` 文件，选择「用其他应用打开 → Aini Player」。

> 升级安装请保留原签名，直接覆盖即可，数据不会丢失。

## 常见问题

**Q：装完打开是空的，没有内容？**
A：本应用不内置任何影视内容，需要自己导入源后才能使用。

**Q：封面不显示？**
A：多为图床校验 Referer 所致。请确认「本地代理」为开启状态，并在设置里重新刷新一次。

**Q：能播放但一直缓冲？**
A：切换解码方式（硬解 / 软解）试试；若仍不行，多半是源本身失效。

**Q：提示「应用未安装」？**
A：旧版本是用别的签名装的，先卸载旧版再安装。

## 免责声明

- 本应用仅为**播放器工具**，不提供、不存储、不分发任何影视资源；
- 所有内容均来自用户自行导入的第三方源，与本项目无关；
- 请勿将本工具用于任何侵犯版权或违反当地法律法规的用途；
- 使用本软件产生的一切后果由使用者自行承担。

## 更新日志

### v1.59.25
- 优化源加载与异常提示
- 修复部分设备海报加载失败
- 播放器稳定性改进

## 反馈

有问题请到 [Issues](../../issues) 提交，附上机型、系统版本和复现步骤，方便定位。
