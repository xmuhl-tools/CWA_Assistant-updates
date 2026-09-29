# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.4.1**（build 24）
- 最近更新：版本 v0.4.1（build 24）— 两处修正：【类型】第一项改名为「帮我问清楚」；修掉一个老用户才会遇到的启动默认值错位。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.4.1-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.1/CWA_Assistant-0.4.1-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.4.1-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.1/CWA_Assistant-0.4.1-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.4.1-win-x64.zip
  73058f5010b6516a97b2a45981e0d8c6fddbdcb295432181ad26cb574621d032
CWA_Assistant-0.4.1-win-x64-Setup.exe
  06b872fdcebee69bd4c4edd6440bb7c7dfb3b633448cea95c9a97bdffd0f4a41
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-29），请勿手工改动。
