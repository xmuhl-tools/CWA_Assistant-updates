# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.3.0**（build 15）
- 最近更新：版本 v0.3.0（build 15）——版本方案切换 + 文档体系重构 + 更新体验增强。

1) 版本方案：改为三段语义化版本 v0.3.0，标题栏显示 v0.3.0 (build 15)；自动更新仍按文件属性第四段 build 比较，已装旧版可正常收到升级提示。
2) 《使用手册》正式降级更名为 README.pdf，帮助框按钮改为【打开 README】；程序目录随包两份文档：《AI方案助手_图解入门.pdf》与 README.pdf。
3) 更新体验增强：替换失败时新版文件保留在 update_pending 目录并生成“一键修复”，关闭程序后双击一次即可完成更新（原先需要手动重新下载）。
4) 能力包升级 1.3.0：项目类方案新增《实施移交清单》（实施范围与验收 / 待开发确认 / 素材附件），示例明示“方案交给程序员实现”。
5) 修复：抓取确认与保存提示词弹窗的只读文本整片高亮（焦点移出编辑框，实心高亮像素归零）；两册手册全面修订（目录页码+点击跳转、章节防孤行、16 张截图按实机重拍）。

程序其余功能无变化。

校验值（SHA-256）：
- CWA_Assistant-0.3.0-win-x64.zip 3715a9b964c4a244c33326bca3d921d03f52ba7d8b4ef61033ed288bf12a28d5
- CWA_Assistant-0.3.0-win-x64-Setup.exe c35c763a3e1f4fe12309bedbb61d1aa78808908eba2c141dbc37b9e4bf7ed601

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.3.0-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.0/CWA_Assistant-0.3.0-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.3.0-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.3.0/CWA_Assistant-0.3.0-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.3.0-win-x64.zip
  3715a9b964c4a244c33326bca3d921d03f52ba7d8b4ef61033ed288bf12a28d5
CWA_Assistant-0.3.0-win-x64-Setup.exe
  c35c763a3e1f4fe12309bedbb61d1aa78808908eba2c141dbc37b9e4bf7ed601
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-23），请勿手工改动。
