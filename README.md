# downkyi

DownKyi **1.6.1 扫码登录修复版**的分发仓库 —— 非官方构建，仓库内不含源码。

下载见 [Releases](https://github.com/hehe1885/downkyi/releases)（附件名 `DownKyi-1.6.2.zip`）。

## 这是什么

- **代码基线是上游最后一版 DownKyi 1.6.1**（2023-12-10 发布），并非官方 1.6.2 发布包
- 修复 **B 站扫码登录无法生成二维码**（`qrcodeKey` 获取失败）的问题
- 包内显示的版本号已被手动改为 1.6.2，**仅作区分标记**，不代表上游发布过 1.6.2
- 请勿把本包的问题反馈给上游作者

## 包内文件

- `DownKyiFix.dll` —— 上述扫码登录修复
- `Make-Login.ps1` —— 手动注入登录凭据生成 `Config\Login`（参数：`-SESSDATA`、`-BILI_JCT`、`-DedeUserID` 等）
- `DownKyi.exe.orig-1.6.1-backup`、`DownKyi.Core.dll.orig-backup` —— 修改前的原始文件备份，便于回退
- `ffmpeg.exe`、`aria2c.exe` —— 随包分发的第三方程序，许可证见 `FFmpeg_LICENSE.txt`、`aria2_COPYING.txt`

## 运行要求

- Windows 10 / 11 x64
- .NET Framework 4.7.2 或更高（若提示缺失，按包内 `打不开DownKyi请点我.txt` 的链接安装）

## 说明

- 已剥离打包者本机的个人数据：配置、登录凭据备份、下载数据库、封面/头图缓存、运行日志
- 本包为个人修改版，**未附带对应源码**
- 原始项目 **DownKyi**（作者 leiurayer），以 **GPL-3.0** 授权，版权归原作者所有：<https://github.com/leiurayer/downkyi>
- 上游已于 2023 年停更，仓库默认分支为 `Deprecated`；上游最后一个版本为 v1.6.1
