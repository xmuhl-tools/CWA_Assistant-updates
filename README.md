# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.2.1.14**（build 14）
- 最近更新：修复自动更新下载偶发挂死（家族性缺陷）：下载读循环新增停滞中止保护——任一下载源 15 秒无字节进展即放弃并换下一源（原实现仅依赖 WinHTTP 逐操作超时，代理"涓流"喂字节时可无限挂死，界面永远停在"正在下载更新"）；程序功能本身无变化。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.2.1.14-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.14/CWA_Assistant-0.2.1.14-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.2.1.14-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.14/CWA_Assistant-0.2.1.14-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.2.1.14-win-x64.zip
  18b9dbaa51193f6bc7ccfce9ca97e17efc7060d6874e585958c2e20f4bf5d545
CWA_Assistant-0.2.1.14-win-x64-Setup.exe
  095c1cdf5671c79e6daf6cfa59c1938eac27166327732e2961e8bbcd58e60ca1
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。
