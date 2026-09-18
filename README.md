# CWA Assistant

更新发布通道：更新清单 + Windows x64 下载包（CWA_Assistant）。

- 当前版本：**0.2.1.9**（build 9）
- 最近更新：提示词预览区重做：预览可直接编辑并作为发送/复制的内容源；新增【复制提示词】与【保存提示词】（可存为 Markdown 文档，供有输入字数限制的本地大模型工具以文件方式提交）；生成不再带出此前问过的问题；提示词自动附带允许跳过无法确认问题的规则。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [CWA_Assistant-0.2.1.9-win-x64-Setup.exe](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.9/CWA_Assistant-0.2.1.9-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [CWA_Assistant-0.2.1.9-win-x64.zip](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.9/CWA_Assistant-0.2.1.9-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\CWA_Assistant`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
CWA_Assistant-0.2.1.9-win-x64.zip
  f7fb2aefcaf0e83a91bebc37b2cb88465ea59dd009a77f44a4fcefacbd26a042
CWA_Assistant-0.2.1.9-win-x64-Setup.exe
  19e40d75f685c5b32231cba79a7652207e08d3b96d66fab7e5a7eec0cd78e69d
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-18），请勿手工改动。
