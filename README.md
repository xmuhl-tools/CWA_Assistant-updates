# CWA Assistant — 发布通道

CWA Assistant 是一个 Windows 绿色（便携）桌面软件：本地能力包 + 会话管理 + Prompt 拼装，经剪贴板桥接到浏览器中的 DeepSeek 等模型网页使用。

本仓库是它的更新发布通道，不是源码仓库：`update.json` 为更新清单（版本、SHA-256、镜像链），Releases 提供各版本安装包。

> Release 页的 "Source code (zip / tar.gz)" 是 GitHub 自动生成的标签快照（无法关闭），不是安装包；请下载 Assets 区的 `CWA_Assistant-<版本>-win-x64.zip`。

## 下载

- 最新版本：https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/latest
- 国内镜像（jsDelivr，同一文件）：https://cdn.jsdelivr.net/gh/xmuhl-tools/CWA_Assistant-updates@v0.2.1.2/CWA_Assistant-0.2.1.2-win-x64.zip

## 安装与使用

1. 解压 zip 到任意可写目录（绿色软件：不写注册表 / AppData，配置与会话都保存在程序目录内）；
2. 双击 `CWA_Assistant.exe`；
3. 按软件内引导使用：绑定浏览器页面 → 输入问题 → 生成 Prompt → 填入浏览器。

系统要求：Windows 10 / 11（x64）。

## 自动更新

程序启动时自动读取本仓库 `update.json` 检查更新：发现新版本弹窗提示（立即更新 / 跳过此版本 / 稍后）；下载包强制 SHA-256 校验，通过并经确认后才替换并重启；任一步失败都不影响当前使用。

## 完整性校验

SHA-256 记录在 `update.json` 的 `sha256` 字段，可自行核对：`certutil -hashfile CWA_Assistant-<版本>-win-x64.zip SHA256`。
