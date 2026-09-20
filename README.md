# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.2.1.12**（build 12）
- 最近更新：面向普通用户的上手改造：主界面新增一句话产品定位与【示例】下拉（日常 6 例 + 项目 3 例，点一下自动填入照着改）；【会话】改名【存档线】并在下拉里直接显示每条线已存的成果数；切换或启动时预览区直接显示这条线的本地记录；任务类型改为用户语言（自动判断（推荐）/做个小工具/做套流程/出套方案/学套方法）；帮助窗口重写并新增两个按钮可直接打开随包的两本手册；修复帮助窗口文字被按钮遮挡、更新弹窗缺少当前版本号等问题。快速上手引导只在首次使用时出现。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.2.1.12-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.12/CWA_Assistant-0.2.1.12-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.2.1.12-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.12/CWA_Assistant-0.2.1.12-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.2.1.12-win-x64.zip
  edf593f64ec8d4c50530792e11f0058cd4a8d2f0f34911d1e275c49ace060587
CWA_Assistant-0.2.1.12-win-x64-Setup.exe
  d62590f49881881aa4bf64a631eba0f5dda51aa9630da62f4007786a9ebab8f6
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-20），请勿手工改动。
