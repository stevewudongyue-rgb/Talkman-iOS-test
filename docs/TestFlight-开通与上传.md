# TestFlight 开通与上传手册（Talk Man iOS）

状态：**待 Steve 完成付费开通**；其余步骤已备好，账号激活当天即可上传。

## 第 1 步（仅 Steve 可做）：加入 Apple Developer Program

1. 用 Mac 打开 https://developer.apple.com/programs/enroll/ ，点「Start your enrollment」
2. 登录 Apple ID（dongyue wu，与 Xcode 里同一个）
3. 选择 **Individual / 个人**（不需要公司 D-U-N-S，最快；App Store 显示个人开发者名）
4. 支付 **$99/年**（支持支付宝/银联信用卡）
5. 等待激活（通常 24—48 小时，邮件通知；此后每年续费一次）

> 开通后同一 Apple ID 所在的 Team 会自动从「Personal Team」升级，Xcode 无需换账号。

## 第 2 步（M2 自动执行）：上传 TestFlight

Steve 确认激活后告知 M2，M2 在公司 Mac 执行（已验证前置条件：麦克风权限描述✓、1024 单尺寸图标✓、版本号可注入✓）：

1. App Store Connect 创建 App 记录（Bundle ID `cn.cololight.talkman.ipad`，名称 Talk Man）
2. Release 归档并注入版本号（0.1.31 / 构建 20261103.x）：
   `xcodebuild archive -configuration Release … && xcodebuild -exportArchive -method app-store …-allowProvisioningUpdates`
3. 上传后 TestFlight 处理约 10—30 分钟
4. 内部测试（最多 100 人，**无需 Beta 审核**，最快）：App Store Connect 添加同事 Apple ID 邮箱 → 对方收邮件 → 装「TestFlight」App → 接受即可安装
5. 外部测试（最多 10000 人，需一次简单 Beta 审核）：生成公开邀请链接，放到本下载页

## 第 3 步：下载页更新

M2 把 TestFlight 邀请链接更新到本仓库 README 的 iOS 区块，替换「自签指引」为首选方案。

## 同事视角（TestFlight 开通后）

收到邀请邮件 → App Store 装 TestFlight → 在 TestFlight 里装 Talk Man → **90 天有效**，新构建上传后 TestFlight 自动提示更新；不再需要连 Mac、不受 7 天限制。

---

*费用与账号归 Steve；上传、测试员管理、下载页维护由 M2 侧负责。自签方案保留为后备。*
