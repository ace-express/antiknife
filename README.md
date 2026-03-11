<p align="center">
  <img src="assets/icon.png" width="128" height="128" alt="AntiKnife Logo">
</p>

<h1 align="center">AntiKnife</h1>

<p align="center">
  <strong>Multi-account manager for Antigravity IDE</strong><br>
  Seamlessly rotate between your Google accounts with zero interruption.
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

## ✨ Features

### 🔄 Automatic Token Rotation
Manage multiple Google accounts and let AntiKnife automatically rotate tokens when quota limits are reached. No more manual switching — just keep coding.

### 📊 Real-Time Quota Monitoring
See your remaining quota at a glance, right in the status bar. Visual indicators show usage across all model families (Gemini Pro, Flash, Claude) so you always know where you stand.

### 👥 Multi-Account Management
- Add accounts via secure Google OAuth2 login  
- Enable/disable individual accounts with one click  
- Drag-and-drop to reorder account priority  
- Automatic IDE account import  

### ⚡ Smart Rotation Strategies
- **Priority-based**: Use your preferred account first, fall back when quota runs low  
- **Per-model tracking**: Separate quota monitoring for each AI model family  
- **Configurable thresholds**: Set when to switch to the next account  

### 🖥️ Intuitive Sidebar Panel
A dedicated sidebar panel gives you full control:
- View all accounts with status and quota  
- Switch active account instantly  
- Monitor rotation status in real-time  
- Access admin settings  

### 🌐 Local & Remote Mode
- **Local mode**: Everything runs on your machine  
- **Remote mode**: Connect to a shared server for team account management  

## 📦 Installation

### From Open VSX Registry

Search for **AntiKnife** in the extension marketplace, or install directly:

```
ext install ace.antiknife
```

### Manual Install

Download the `.vsix` file from [Releases](https://github.com/ace-express/antiknife/releases), then:

```bash
# In Antigravity IDE / VSCodium
code --install-extension antiknife-x.x.x.vsix
```

## 🚀 Getting Started

1. Install AntiKnife from the extension marketplace  
2. Click the **🔪 knife icon** in the activity bar  
3. Click **Add Account** to sign in with your Google account  
4. Add more accounts as needed  
5. Click **Enable** to start automatic rotation  

## 🔧 Requirements

- Antigravity IDE v1.85.0 or later (or any compatible VS Code fork)

## 🐛 Found a Bug?

Please [open an issue](https://github.com/ace-express/antiknife/issues/new?template=bug_report.md) with steps to reproduce.

## 💡 Feature Requests

Have an idea? [Submit a feature request](https://github.com/ace-express/antiknife/issues/new?template=feature_request.md).

## 📄 License

AntiKnife is proprietary software. See [LICENSE](LICENSE) for details.

---

<p align="center">
  Made with ❤️ for the Antigravity IDE community
</p>
