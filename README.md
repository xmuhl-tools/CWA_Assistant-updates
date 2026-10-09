# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.4.5**（build 28）
- 最近更新：版本 v0.4.5（build 28）— 提问有效性与网页下一步指引修订版：改了需求之后旧提问不会再被发出去、载入既有记录时类型会跟着恢复、填入网页前会再次确认目标窗口还是不是它、更新过程中点取消不会再走进安装确认，另把「存成的提问文件怎么交给网页模型」说清楚了。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.4.5-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.5/CWA_Assistant-0.4.5-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.4.5-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.5/CWA_Assistant-0.4.5-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.4.5-win-x64.zip
  f4a78309d11636cfc5f00e58bbb3b2c47e03f8706b240db366e0be735665ce9a
CWA_Assistant-0.4.5-win-x64-Setup.exe
  739f9c120c4ce329a40f998b5ca7a7f2139c1259223cdac09164957bfdfd5dea
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-10-09），请勿手工改动。
