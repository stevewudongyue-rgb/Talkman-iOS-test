# Talk Man · 下载与安装

语音转文字 → AI 整理／改写／翻译 → 一键填入电脑输入框。iPhone／iPad 应用＋Mac 伴侣（iOS 伴侣）＋（家用）Desktop 桌面版。

## macOS · iOS 伴侣（配 iPhone／iPad 应用）

| 下载 | 说明 |
|---|---|
| [安装镜像 DMG（Apple Silicon）](downloads/TalkMan-iOS伴侣-macOS-AppleSilicon.dmg) | 推荐：打开后把「TalkMan iOS 伴侣」拖进 Applications 文件夹 |
| [ZIP 打包](downloads/TalkMan-iOS伴侣-macOS-AppleSilicon.zip) | 解压即用 |

- 无须安装 Python；Apple Silicon（M 系列芯片）Mac，macOS 13+。
- **首次打开如被系统阻拦**（未做 Apple 公证）：右键 App 选「打开」，或到「系统设置 → 隐私与安全性」点「仍要打开」。仅从本页面下载。
- 使用步骤：打开 App → 电脑模型设置里填千问 Key → 启用 iPad/iPhone 连接 → 手机 Talk Man 设置粘贴配对串并连接。
- 需要「填入电脑」功能时：系统设置 → 隐私与安全性 → **辅助功能** → 添加并允许「TalkMan iOS 伴侣」，然后退出重开 App。
- 版本：0.1.31（构建 20261108，nothing 风格界面＋在线检查更新＋跨焦点填入修复），协议支持语序分行／选区移动／选区翻译。

## iPhone／iPad 应用（Talk Man）

iOS 应用受 Apple 签名机制限制，**不能像 Mac 一样直接下载安装**，目前两条路：

1. **TestFlight（推荐，开通中）**：同事点一个链接即可安装，无需连线电脑，构建 90 天有效。管理员加入 Apple Developer Program 后约 1—2 天激活，届时这里会放加入链接（[开通进度与手册](docs/TestFlight-开通与上传.md)）。
2. **公司 Mac 自签（现在就能用）**：用公司 Mac ＋ 自己的免费 Apple ID，Xcode 编译安装到自己的 iPhone，**签名 7 天有效**需续签。步骤见 [iOS-自签安装指引](docs/iOS-自签安装指引.md)。

## Desktop 桌面版（家用机维护）

见私有仓库 `Talkman` 的 Releases（desktop-v0.1.x）。此处不放公开镜像；如需公开入口请与管理员确认。

---

*本页面由公司 M2 侧构建与维护；Talk Man 产品与源码归 Steve 所有。*
