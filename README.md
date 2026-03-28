<p align="center">
  <img src="assets/icon.png" width="128" height="128" alt="AntiKnife Logo">
</p>

<h1 align="center">AntiKnife</h1>

<p align="center">
  <strong>Multi-account manager & Network Optimizer for Antigravity IDE</strong><br>
  Seamlessly rotate between your Google accounts with zero interruption and establish rock-solid connections.
</p>

<p align="center">
  <a href="README.zh-CN.md">🌐 中文</a> | <strong>English</strong>
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

## ✨ Highlights

1. **Seamless Account Switching & Rotation** — Switch between Google accounts instantly with zero IDE restart required. Automatically rotate tokens when your current account's quota runs low to keep your flow uninterrupted.
2. **Network Enhancement** — Features a robust streaming proxy that significantly mitigates EOF drops. Tailor your network settings to help navigate firewalls and interruptions for a more stable streaming connection.
3. **Team Authorization** — Distribute a massive pool of tokens across an entire team via an exclusive remote mode and admin dashboard without ever sharing the underlying credentials.
4. **Real-Time Quota Monitoring** — See your remaining limits and usage directly in the status bar across all model families (Gemini Pro, Flash, Claude), with color-coded alerts and countdowns.

## 🚀 Features

### ✨ 1. Seamless Account Switching
- **Zero-restart:** Quickly switch between multiple active Google accounts on the fly.
- **Auto-Rotation:** Let AntiKnife passively rotate to the next pooled account when you hit quota boundaries. 
- **Pool Management:** Add, group, and securely authorize active Google accounts into your available pool.

### 🌐 2. Network Enhancement & Tweaks
- **Network Optimization:** Custom Gemini streaming proxy tailored to significantly reduce mid-stream interrupts and network drops commonly seen from firewalls.
- **Granular Net Control:** Easily toggle Fast, Stable, and Legacy networking presets, or fine-tune advanced connection and heartbeat strategies straight from the IDE settings to match your specific latency requirements.

### 🔑 3. Team Authorization & Remote Mode
- **Remote Server Connections:** Connect to a remote team server via client keys. Administrators can securely distribute shared tokens natively.
- **Built-in Admin Panel:** Manage your organization, allocate tokens securely with limits, and track per-member limits directly inside an integrated UI dashboard.

### 📊 4. Real-Time Quota Display
- **Status Bar Integration:** Instantly verify your remaining queries for Claude, Gemini Pro, and Gemini Flash right in your IDE.
- **Detailed Metrics:** Progress bars visualize utilization, tier boundaries, and the next limit reset timer.
- **Custom Threshold Settings:** Decide exactly when AntiKnife warns you or autorotates (0% - 80%).

![Local mode — accounts](assets/screenshots/local_accounts.png)

![Remote mode — team](assets/screenshots/remote_accounts.png)

## 📦 Installation

### From Open VSX Registry
Search for **AntiKnife** in the extension marketplace, or install directly:
```bash
ext install ace.antiknife
```

### Manual Install
Download the `.vsix` file from [Releases](https://github.com/ace-express/antiknife/releases), then:
```bash
# In Antigravity IDE / VSCodium
code --install-extension antiknife-x.x.x.vsix
```

## 🚀 Getting Started

1. Install AntiKnife from the extension marketplace.
2. Click the 🔪 knife icon in the activity bar.
3. Your IDE's current Google account is auto-imported.
4. Click **Add Account** to sign in with additional Google accounts.
5. In Settings, enable **Account Rotation** for passive management, and **Network Enhancement** for optimal streaming.

## 💻 Supported Platforms

| OS | Architecture | VSCE Target |
|----|-------------|-------------|
| macOS | Apple Silicon (ARM64) | `darwin-arm64` |
| macOS | Intel (x64) | `darwin-x64` |
| Linux | x64 | `linux-x64` |
| Linux | ARM64 | `linux-arm64` |
| Windows | x64 | `win32-x64` |
| Windows | ARM64 | `win32-arm64` |

## 🔧 Requirements
- Antigravity IDE v1.85.0 or later

## 🐛 Found a Bug?
Please [open an issue](https://github.com/ace-express/antiknife/issues/new?template=bug_report.md) with steps to reproduce.

## 📄 License

AntiKnife is proprietary software. See [LICENSE](LICENSE) for details.

---

<p align="center">
  Made with ❤️ for the Antigravity IDE community
</p>
