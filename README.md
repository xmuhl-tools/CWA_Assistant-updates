# AI 方案助手 — 发布通道

AI 方案助手 是一个 Windows 绿色（便携）桌面软件：本地能力包 + 会话管理 + 提示词拼装，经剪贴板桥接到浏览器中的 DeepSeek 等模型网页使用。

本仓库是它的更新发布通道，不是源码仓库：`update.json` 为更新清单（版本、SHA-256、镜像链），Releases 提供安装包与便携包。

> Release 页的 "Source code (zip / tar.gz)" 是 GitHub 自动生成的标签快照（无法关闭），不是安装包；请下载 Assets 区的文件。

当前版本：**v0.2.1.7**（build 7），更新内容见对应 Release 说明。

## 下载

- **安装版（推荐）**：`CWA_Assistant-<版本>-win-x64-Setup.exe` —— 双击安装，桌面自动创建快捷方式
- **便携版**：`CWA_Assistant-<版本>-win-x64.zip` —— 解压到任意可写目录，双击 `CWA_Assistant.exe`
- 国内镜像（jsDelivr，宿主为版本标签）：`https://cdn.jsdelivr.net/gh/xmuhl-tools/CWA_Assistant-updates@v<版本>/CWA_Assistant-<版本>-win-x64.zip`

## 安装与使用

1. 运行 `CWA_Assistant-<版本>-win-x64-Setup.exe`，按向导操作：在"选择安装位置"页可点"浏览…"修改目录（默认在用户目录下），按需勾选"创建桌面快捷方式"；
2. 若系统提示"Windows 已保护你的电脑"，点"更多信息 → 仍要运行"；
3. 按软件内引导使用：绑定浏览器页面 → 输入问题 → 生成 Prompt → 填入浏览器。详见安装目录下的《CWA_Assistant_使用手册.pdf》。

系统要求：Windows 10 / 11（x64）。安装与运行都不需要管理员权限，程序本身不写注册表。安装包版可在系统"应用和功能"里一键卸载（只移除程序文件，会话与设置保留在安装目录，想彻底清除再手动删除目录）；便携版卸载 = 删除解压目录。

## 自动更新

程序启动时自动读取本仓库 `update.json` 检查更新：发现新版本弹窗提示（立即更新 / 跳过此版本 / 稍后）；更新清单带 RSA-2048 数字签名，客户端验证通过才会采信，签名不符或缺失一律拒绝；下载包强制 SHA-256 校验，通过并经确认后才替换并重启；任一步失败都不影响当前使用。

## 完整性校验

`update.json` 的 `sha256` 字段是更新包（zip）的校验值，安装包的校验值写在对应 Release 的说明里。核对方法：

```text
certutil -hashfile CWA_Assistant-<版本>-win-x64.zip SHA256
```
