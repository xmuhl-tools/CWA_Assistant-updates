# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.4.0**（build 23）
- 最近更新：版本 v0.4.0（build 23）— 去掉一个用不上的【类型】选项，示例下拉会帮你自动切类型；另修复一个会毁掉存档记录的严重缺陷。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.4.0-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.0/CWA_Assistant-0.4.0-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.4.0-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.4.0/CWA_Assistant-0.4.0-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.4.0-win-x64.zip
  e01c7942b8922806a4c29415e0dfee238b1882cb99706f93bea14d0855cf8462
CWA_Assistant-0.4.0-win-x64-Setup.exe
  4129b0e28174f44146cdca84e07c8e3f1ca236e4587162de263781d41ac10641
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-29），请勿手工改动。
