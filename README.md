# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.2.1.13**（build 13）
- 最近更新：说明文档全面复核修订：《使用手册》修正入门手册案例数（7 处改为 9）、目标窗口未绑定状态描述、存档线视图内容说明、目录结构补全图解入门手册、卸载与故障排查措辞等 8 处；《AI方案助手_图解入门》全部截图按 0.2.1.13 实机重新采集；仓库 README 同步修订（安装器注册表行为说明、设置项列表、存档线叫法统一等）。程序功能本身无变化。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.2.1.13-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.13/CWA_Assistant-0.2.1.13-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.2.1.13-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.13/CWA_Assistant-0.2.1.13-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.2.1.13-win-x64.zip
  1a50af76aca098111dcee3dd6217d662639be6e756d8f9920d5e688b87733c7e
CWA_Assistant-0.2.1.13-win-x64-Setup.exe
  64fc08ca740d74bc8d31d304b4334bd1ec65cb1b94948051bcef757f21865d2b
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。
