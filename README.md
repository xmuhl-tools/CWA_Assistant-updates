# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.3.4**（build 19）
- 最近更新：版本 v0.3.4（build 19）——修复"程序开着时切换分辨率，主窗口不再自适应"的问题。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.3.4-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.4/CWA_Assistant-0.3.4-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.3.4-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.4/CWA_Assistant-0.3.4-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.3.4-win-x64.zip
  b36052d6a39a135c0f0bf39c0347afc78e50d5dc39212de429058946e5721bae
CWA_Assistant-0.3.4-win-x64-Setup.exe
  333332ca21491217fbde08bffaf0d8b278154175777ae3c439a009e421e547f2
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-24），请勿手工改动。
