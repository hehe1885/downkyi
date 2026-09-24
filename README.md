# downkyi

DownKyi 1.6.2 的**个人修复版**分发仓库 —— 非官方构建，仓库内不含源码。

本仓库只用于分发一个可直接运行的 Windows 绿色包，下载见 [Releases](https://github.com/hehe1885/downkyi/releases)。

## 包内说明

- 基于 DownKyi 1.6.2 发布包
- 附登录相关修复文件：`DownKyiFix.dll`、`Make-Login.ps1`
- 保留原始文件备份：`DownKyi.exe.orig-1.6.1-backup`、`DownKyi.Core.dll.orig-backup`
- 已剥离打包者本机的个人数据：配置、登录凭据备份、下载数据库、封面/头图缓存、运行日志

## 运行要求

- Windows 10 / 11 x64
- .NET Framework 4.7.2 或更高版本（若提示缺失，按包内 `打不开DownKyi请点我.txt` 的链接安装）

## 第三方与许可

- `ffmpeg.exe`、`aria2c.exe` 为随包分发的第三方程序，许可证见 `FFmpeg_LICENSE.txt`、`aria2_COPYING.txt`
- DownKyi 上游项目以 GPL-3.0 授权，版权归原作者所有：<https://github.com/nilaoda/DownKyi>
- `.orig-backup` 文件为修改前的原始文件备份，便于回退
