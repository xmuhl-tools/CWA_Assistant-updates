# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.3.3**（build 18）
- 最近更新：版本 v0.3.3（build 18）——低分屏窗口适配修复 + 发布流程固化。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.3.3-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.3/CWA_Assistant-0.3.3-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.3.3-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.3/CWA_Assistant-0.3.3-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.3.3-win-x64.zip
  1b7a4b515b583b84f61fdca00bc5c179746e24c34dccad82f40565ecbd4e191a
CWA_Assistant-0.3.3-win-x64-Setup.exe
  f2c3702887032e0e2b6b4d5bac6ad1107847c7303fee264ca3dfe836cb8a52cc
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-23），请勿手工改动。
