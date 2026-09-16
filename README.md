# CWA Assistant — 发布通道

CWA Assistant 是一个 Windows 绿色（便携）桌面软件：本地 Prompt 能力包 + 会话管理 + Prompt 拼装，经剪贴板桥接到浏览器中的 DeepSeek 等模型网页使用。

本仓库是它的**更新发布通道**，不是源码仓库。仓库内容只有两类：

- `update.json` —— 更新清单（版本号 / 构建号 / SHA-256 校验值 / 下载镜像链），由程序启动时自动读取；
- Releases —— 各版本的安装包 `CWA_Assistant-<版本>-win-x64.zip`。

> **注意**：Release 页面里的 **"Source code (zip / tar.gz)"** 是 GitHub 对每个版本自动生成的
> 标签快照（无法关闭），不是本软件的安装包。请下载 **Assets** 区里的
> `CWA_Assistant-<版本>-win-x64.zip`。

## 下载

- 最新版本：[Releases / latest](https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/latest)
- 直链（v0.2.1.2）：
  `https://github.com/xmuhl-tools/CWA_Assistant-updates/releases/download/v0.2.1.2/CWA_Assistant-0.2.1.2-win-x64.zip`
- 国内镜像（jsDelivr CDN，同一文件）：
  `https://cdn.jsdelivr.net/gh/xmuhl-tools/CWA_Assistant-updates@v0.2.1.2/CWA_Assistant-0.2.1.2-win-x64.zip`

## 安装与使用

1. 下载 zip，解压到任意可写目录（绿色软件：不写注册表 / AppData，配置与会话都保存在程序目录内）；
2. 双击 `CWA_Assistant.exe` 运行；
3. 按软件内引导使用：绑定浏览器页面 → 输入问题 → 生成 Prompt → 填入浏览器。

系统要求：Windows 10 / 11（x64）。

## 自动更新

程序启动时会自动读取本仓库的 `update.json` 检查新版本：发现更新会弹窗提示
（立即更新 / 跳过此版本 / 稍后）。

- 下载的更新包**强制 SHA-256 校验**（与清单比对，不符即弃包换源）；
- 校验通过并经你确认后，才会退出程序、替换文件并自动重启；
- 任何一步失败都不会影响当前程序的使用，也可随时到本仓库手动下载。

无需手动检查更新。

## 完整性校验

每个版本的 SHA-256 记录在仓库根目录 `update.json` 的 `sha256` 字段，
下载后可用 `certutil -hashfile CWA_Assistant-<版本>-win-x64.zip SHA256` 自行核对。
