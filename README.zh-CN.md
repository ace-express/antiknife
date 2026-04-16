<p align="center">
  <img src="assets/icon.png" width="128" height="128" alt="AntiKnife Logo">
</p>

<h1 align="center">AntiKnife</h1>

<p align="center">
  <strong>专为 Antigravity IDE 打造的多账号管理与网络增强工具</strong><br>
  在多个 Google 账号之间无缝轮换，享受极致稳定的流式连接，零中断编码。
</p>

<p align="center">
  <strong>中文</strong> | <a href="README.md">English</a>
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

## 核心亮点

1. **无感账号切换** -- 零重启，在多个 Google 账号之间即时切换。当前账号额度不足时，自动静默轮换到下一个可用账号，编码流程不中断。
2. **第三方模型接入** -- 自带 API Key，接入任意兼容 OpenAI 的 LLM 提供商。可在同一面板中同时管理 Google 账号和 GPT、DeepSeek 等第三方模型。
3. **网络增强** -- 内置流式传输代理，专门针对 EOF 中断和流式断连进行优化。支持多种连接策略预设，即使在严苛的防火墙环境下也能保持稳定连接。
4. **实时额度监控** -- 在状态栏直接展示所有模型系列（Claude / Gemini Pro / Gemini Flash）的剩余额度百分比，悬停查看逐模型进度条与重置倒计时。
5. **团队授权** -- 通过专属 Remote 模式和管理后台，将共享 Token 池分发给整个团队，无需暴露底层凭证。

## 功能特性

### 1. 账号切换与自动轮换

- **零重启切换：** 随时在多个 Google 账号之间即时切换，无需重启 IDE。
- **自动轮换：** 当活跃账号的额度低于设定阈值时，自动静默切换到池中下一个可用账号。
- **账号池管理：** 导入、排序、启用或禁用账号，支持可视化拖拽操作。

![本地模式 -- 账号池管理，逐模型额度条与等级徽章](assets/screenshots/local_accounts.png)

### 2. 第三方模型接入

- **自带 Key 接入：** 填写 API 端点 URL、API Key 和模型名称，即可接入任意兼容 OpenAI 的提供商（OpenAI / DeepSeek / Groq 等）。
- **统一管理：** 在同一侧栏面板中添加、编辑、启用或禁用第三方提供商，与 Google 账号并列管理。
- **自动路由：** 启用第三方提供商后，请求自动转发至该提供商，无需额外手动配置。

![第三方提供商 -- 管理外部 LLM 端点](assets/screenshots/provider.png)

### 3. 网络增强

- **流式代理：** 内置专为 Gemini 流式传输定制的本地代理，大幅减少流中断和连接丢失。
- **连接预设：** 提供极速、稳定、兼容等多种网络预设方案，也支持自定义连接参数和保活策略以适配特殊网络环境。
- **联动自动轮换：** 网络增强与账号轮换协同工作 -- 连接失败时先以优化参数重试，再回退到下一个账号。

![网络增强与自动轮换设置](assets/screenshots/network_enhance_auto_rotation.png)

### 4. 实时额度显示

- **状态栏集成：** 无需离开编辑器，一眼看清 Claude、Gemini Pro、Gemini Flash 的剩余额度百分比。
- **悬浮详情面板：** 等宽对齐的逐模型额度百分比、进度条和重置倒计时。
- **可配置阈值：** 自定义在额度降至多少百分比（0% -- 80%）时触发预警或自动轮换。

![额度详情悬浮窗 -- 逐模型额度条与重置倒计时](assets/screenshots/quota.png)

### 5. 团队授权与远程模式

- **远程服务器连接：** 通过 Tenant ID 和 Client Key 接入中心化团队服务器，客户端无需手动管理 Token。
- **管理后台：** 管理 Token 池、分配客户端席位、设置有效期策略，并在集成面板中监控成员用量。

![远程模式 -- 团队服务器连接](assets/screenshots/remote_accounts.png)

## 安装说明

### 从 Open VSX 安装

在扩展市场搜索 **AntiKnife** 进行安装，或执行：
```bash
ext install ace.antiknife
```

### 手动安装

从 [Releases](https://github.com/ace-express/antiknife/releases) 下载 `.vsix` 文件后导入：
```bash
code --install-extension antiknife-x.x.x.vsix
```

## 快速开始

1. 从扩展市场安装 AntiKnife。
2. 点击活动栏中的 AntiKnife 图标，打开管理面板。
3. IDE 当前登录的 Google 账号会被自动导入。
4. 点击 **Add Account** 授权绑定更多 Google 账号到账号池。
5. 在 Settings 中开启**账号轮换**实现自动切号，开启**网络增强**优化流式传输稳定性。

## 支持平台

| 操作系统 | 架构 | VSCE 构建目标 |
|---------|------|-------------|
| macOS | Apple Silicon (ARM64) | `darwin-arm64` |
| macOS | Intel (x64) | `darwin-x64` |
| Linux | x64 | `linux-x64` |
| Linux | ARM64 | `linux-arm64` |
| Windows | x64 | `win32-x64` |
| Windows | ARM64 | `win32-arm64` |

## 环境要求

- Antigravity IDE v1.85.0 及以上版本

## 问题反馈

发现 Bug 或有改进建议，欢迎在 [GitHub 仓库](https://github.com/ace-express/antiknife/issues) 提交 Issue。

## 许可证

AntiKnife 专有闭源协议 -- 详见 [LICENSE](LICENSE)。

---

<p align="center">
  Made for the Antigravity IDE community
</p>
