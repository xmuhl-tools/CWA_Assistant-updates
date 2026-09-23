# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.3.1**（build 16）
- 最近更新：版本 v0.3.1（build 16）——人工验收三项修订：更新弹窗更清爽、【帮助】按钮归位、示例回归一句话。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.3.1-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.1/CWA_Assistant-0.3.1-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.3.1-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.1/CWA_Assistant-0.3.1-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.3.1-win-x64.zip
  cf4ac80280fd4ebc052a525d73b497539d3481c5a45f7e8ca085076117772019
CWA_Assistant-0.3.1-win-x64-Setup.exe
  87adfd18df3a6c7429376f10272f19e6dc80f74af1a8e62e6a198885e0beded3
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-23），请勿手工改动。
