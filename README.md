# RhineNetEase-win32-x64

界面与美术来自 **RhinE**（原作者：<https://github.com/ericzhang12111-cell/RhinE>），版权归原作者所有。

本仓库只做了一件事：把**网易云音乐在线播放**接入这套主题界面，并发布构建产物。

## 下载

到 [Releases](../../releases) 下载最新压缩包，解压后运行 `RhineNetEase.exe`。

登录态、缓存与日志保存在 `%APPDATA%\RhineNetEase`，不会写进程序目录。

## Credits / 版权

- 界面与美术：**RhinE** — <https://github.com/ericzhang12111-cell/RhinE>
  （MIT License，© the Audio Archive authors；许可原文随安装包附带）
- 本项目只负责把 RhinE 的 foobar2000 面板移植到 Electron，并接入网易云音乐在线播放。
  未获得原作者背书，与原作者无关。
- 如原作者认为本页面引用不妥，请通过 Issue 联系，会立即修改或撤下。

## 改动范围

- Electron 宿主与兼容层（`renderer/shim.js`）；
- 网易云登录、曲库、在线播放接入（本地接口服务）；
- 主题侧少量适配：壁纸宿主 API、标签换行、导轨着色缓存、单张磁带外壳与标签色等。

## 现状说明

这个适配比较粗糙：主题渲染、曲库加载和部分交互仍有不少问题（接口限流时可能加载失败，个别布局细节也未对齐），后续会继续修。