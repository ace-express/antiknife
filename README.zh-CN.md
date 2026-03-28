<p align="center">
  <img src="assets/icon.png" width="128" height="128" alt="AntiKnife Logo">
</p>

<h1 align="center">AntiKnife</h1>

<p align="center">
  <strong>专为 Antigravity IDE 打造的多账号无感管理与网络增强工具</strong><br>
  在多个 Google 账号之间无缝轮换，享受极致流畅的串流环境，零打断编码。
</p>

<p align="center">
  <strong>中文</strong> | <a href="README.md">🌐 English</a>
</p>

<p align="center">
  <a href="https://open-vsx.org/extension/ace/antiknife">
    <img src="https://img.shields.io/badge/Open%20VSX-Install-blue?logo=eclipse-ide" alt="Open VSX">
  </a>
  <a href="https://github.com/ace-express/antiknife/issues">
    <img src="https://img.shields.io/github/issues/ace-express/antiknife" alt="GitHub Issues">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/license-Proprietary-red" alt="License">
  </a>
</p>

---

## ✨ 核心亮点

1. **无感账号切换 (Seamless Account Switching)** — 零重启，即刻在多个 Google 账号间无缝切换，并在额度耗尽时自动无感轮换下一个账号。
2. **网络优化 (Network Enhancement)** — 强大的底层流式网络代理配置，大幅缓解因防火墙或连接不稳导致的串流中断，提供更优的连接体验。
3. **团队授权 (Team Authorization)** — 跨设备团队资源共享，支持通过特定的 Remote 模式分发共用额度和鉴权，免去个人维护的麻烦。
4. **账号额度展示 (Real-Time Quota Display)** — 实时追踪并在状态栏直观展示所有大模型（Gemini Pro / Flash / Claude）的剩余调用额度及重置倒计时。

## 🚀 功能特性

### ✨ 1. 无感账号切换
- **零重启切换:** 随时随地跨账号无感热切换，一键生效，无需繁琐重启 IDE。
- **自动智能轮换:** 让 AntiKnife 成为您的专属管家。针对高频使用者，它会在检测到当前账号额度触底时，自动平滑轮换近乎无限的备用池。
- **本地池管理:** 轻松导入您的所有 Google 账号，提供拖拽排序、自由启用/禁用的灵活手段。

### 🌐 2. 网络定制与增强优化
- **专属流式优化:** 内置专为流传输定制的本地代理机制，有效缓解流中断等常见连接问题。
- **高级自定义:** 提供对开发者友好的网络进阶设置选项，允许您根据实际网络质量自主微调数据传输与保活策略，适应极端特殊的网络状况。

### 🔑 3. 团队授权管控
- **中心化连接系统:** 专属内置 Remote Mode 接入内部或者三方的中心化团队服务器。
- **授权即用:** 管理员可统一安排上传、共享管理 Token 池，将生成的专属 Client Key 下发；开发者只用输入 Key 即可开箱即用。
- **内置管控后台:** 管理员具有专属 Web 面板，随时下发或注销授权权限，统计组成员用量。

### 📊 4. 账号额度实时展示
- **无缝状态栏整合:** 无需跳转打开系统浏览器，一抬头即可看清模型当下的配额用量情况。
- **可视化悬浮仪表板:** 悬停查看多模型的用量百分比进度条与动态重置倒计时，全面掌握消耗水平。
- **自适应阈值提醒:** 自定义轮换与提醒的安全警告线（0% - 80% 可调）。

![本地模式 — 管理账号，逐模型配额条、等级徽章与优先级排序](assets/screenshots/local_accounts.png)

![远程模式 — 团队模式](assets/screenshots/remote_accounts.png)

## 📦 安装说明

### 从 Open VSX 安装
在扩展市场搜索 **AntiKnife** 进行安装，或执行：
```bash
ext install ace.antiknife
```

### 手动安装
从 [Releases](https://github.com/ace-express/antiknife/releases) 下载 `.vsix` 文件后导入：
```bash
# 在终端中执行
code --install-extension antiknife-x.x.x.vsix
```

## 🚀 快速开始

1. 从扩展市场安装 AntiKnife
2. 点击应用活动栏的 🔪 图标，即可打开面板
3. 你的 IDE 当前登录账号会被自动导入工具
4. 点击 **Add Account** 开始授权绑定并引入所有的 Google 账号加入账号池
5. 在左侧面板 Settings 设置项中，开启 **账号轮换** 来享受跨号，开启 **网络增强** 体验代理输出的稳定。

## 💻 支持平台

| 操作系统 | 架构 | VSCE 构建目标 |
|---------|------|----------|
| macOS | Apple Silicon (ARM64) | `darwin-arm64` |
| macOS | Intel (x64) | `darwin-x64` |
| Linux | x64 | `linux-x64` |
| Linux | ARM64 | `linux-arm64` |
| Windows | x64 | `win32-x64` |
| Windows | ARM64 | `win32-arm64` |

## 🔧 环境要求
- Antigravity IDE v1.85.0 及以上版本

## 🐛 问题反馈
如果你发现了 Bug 或是对工具有任何改进建议，欢迎提交 Issue 至 [GitHub 仓库](https://github.com/ace-express/antiknife/issues)。

## 📄 许可证
AntiKnife 专有权闭源协议许可 — 详情请阅读目录下的 [LICENSE](LICENSE) 文档。

---

<p align="center">
  Made with ❤️ for the Antigravity IDE community
</p>
