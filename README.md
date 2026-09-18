# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.2.1.8**（build 8）
- 最近更新：安装包改进：卸载时会询问是否连同用户数据（配置、会话记录与日志）一起删除，默认保留；静默/自动化卸载可用 /DELETEUSERDATA 参数直接删除。程序功能无变化。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.2.1.8-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.8/CWA_Assistant-0.2.1.8-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.2.1.8-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.8/CWA_Assistant-0.2.1.8-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.2.1.8-win-x64.zip
  cee9b68787b78291bd7dc2fef48ee9e1b0d2489dccaca4903f98a564103ef370
CWA_Assistant-0.2.1.8-win-x64-Setup.exe
  0d297fab548beabd2984e365d60b53f12d1ec6704569cc08f20492b78e4e180f
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-18），请勿手工改动。
