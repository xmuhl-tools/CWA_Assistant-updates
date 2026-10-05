# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.4.4**（build 27）
- 最近更新：版本 v0.4.4（build 27）— 示例增强 + 发送更可靠版：手上有现成的范本（截图、Word/PDF 模板、别人的方案）时，新增的示例会让模型先把它拆解清楚、你确认后再照着做一份；同时修复了“点过网页开关后自动发送落空”的问题。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.4.4-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.4/CWA_Assistant-0.4.4-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.4.4-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.4/CWA_Assistant-0.4.4-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.4.4-win-x64.zip
  2050431d6fd8de6401ffaad7ecc564ca53b023f1c16adf75592bcd9ccb3b2cc1
CWA_Assistant-0.4.4-win-x64-Setup.exe
  4f1dc27bf7d147ff06ce815b4f461c3bc29406b867044ee400a08b1b7cacfcd7
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-10-05），请勿手工改动。
