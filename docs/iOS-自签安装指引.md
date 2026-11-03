# iPhone／iPad 版 Talk Man 自签安装指引（公司 Mac）

适用：同事想在自己的 iPhone/iPad 上使用 Talk Man，且暂未开通 TestFlight。
前提：设备系统 iOS/iPadOS 17 以上；愿意每约 7 天重连一次 Mac 续签。

## 一次配好（约 10 分钟，可请 M2 侧代做）

1. 公司 Mac 已装完整 Xcode 与工程源码（GitHub 私有仓 TalkMan-iOS，需管理员邀请）。
2. 在 Xcode「Settings → Accounts」登录**你自己的 Apple ID**（免费账号即可）。
3. USB 连接你的 iPhone，解锁并信任电脑；首次会提示开启「开发者模式」（设置 → 隐私与安全性 → 开发者模式 → 打开 → 重启）。
4. 打开工程，选择 TalkMan target → Signing & Capabilities → 勾自动签名 → 选你的 Personal Team。
5. 顶部选择你的设备，点运行；安装后按提示在「设置 → 通用 → VPN与设备管理」里信任你的开发者证书。

## 日常使用

- Mac 上打开「TalkMan iOS 伴侣」，启用连接并复制配对串；手机 Talk Man 设置里粘贴一次后即锁定，之后点「连接」即可。
- 手机端界面、录音、翻译、语序分行等所有功能与主测试机一致。

## 每 7 天续签（约 2 分钟）

免费签名 7 天过期，App 会无法打开（数据不丢）：USB 连 Mac → Xcode 顶部选你的设备 → 点运行（覆盖安装）→ 手机上即可再用。

## 常见问题

- **安装时提示"team has no devices"**：手机未开开发者模式或未解锁，按第 3 步处理。
- **打开就闪退/提示不受信任**：第 5 步的信任没做，或签名已过期，续签即可。
- **填入电脑没反应**：Mac 辅助功能里没加「TalkMan iOS 伴侣」，加上并退出重开。

---

*该指引与交接文档《TalkMan-Mac部署测试交接.md》同步维护；问题找 M2 侧（公司 Mac）。*
