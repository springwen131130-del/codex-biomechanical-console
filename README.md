# CODEX 生物机械控制台 / CODEX Biomechanical Console

**我们没有给 Codex 换皮肤，而是为它重新做了一台控制台。**

未来的工作不该无聊。让每一次对话、运行、等待和完成，都像在操纵一台真正的生物机械装置。

在视觉设计上，它致敬我最爱的《暗黑破坏神》，也致敬 H.R. 吉格笔下诡异、冷峻而充满生命感的生物机械美学。

**这不是游戏，也不是概念图。**

它是一款连接真实 Codex、可独立启动的第三方本地 AI 控制台。安装完成后，不需要预先打开 Codex Desktop，可直接从桌面入口进入。

**We did not reskin Codex. We built a new control console for it.**

The future of work should not feel boring. Every conversation, run, wait, and completion should feel like operating a real biomechanical machine.

Its visual design is a personal tribute to the dark fantasy of *Diablo* and the strange, cold, living biomechanical art of H. R. Giger.

**This is not a game or a concept render.**

It is an independently launched third-party local AI control console connected to real Codex. After installation, you can open it directly from the desktop without starting Codex Desktop first.

> 本项目不修改 Codex Desktop，也不公开核心接入源码。
>
> This project does not modify Codex Desktop and does not publish its private integration source code.

## 界面一览 / Console Overview

![CODEX Biomechanical Console overview](./01-console-overview.png)

- **左侧 / Left:** Codex 对话与输入区 / Codex chat and composer.
- **中间 / Center:** 动态主题藏品区 / animated themed collection.
- **右侧 / Right:** 设置、预览和辅助信息屏 / settings, previews, and auxiliary information.
- **底部 / Bottom:** 新对话、搜索、插件、自动化、项目和预览快捷入口 / shortcuts for chat, search, plugins, automations, projects, and preview.

## 常用交互 / Essential Controls

### 1. 主题藏品切换 / Theme Collection Switch

![Theme and collection switch](./02-skin-and-collection-switch.png)

点击中下方的核心按钮，会循环切换中心动态藏品以及与它配套的整套主题外壳。

Click the lower-center core control to cycle both the animated center collection and its matching shell theme.

### 2. 设置是两步操作 / Settings Use a Two-Step Flow

![Settings two-step flow](./03-settings-two-step.png)

先点击左下发光设置节点，再在右侧辅助屏选择界面语言、输入字号、模型、推理强度等选项。语言和字号选择会被记住。

First click the glowing Settings node in the lower-left corner, then choose language, input size, model, reasoning effort, and other options on the right auxiliary screen. Language and font-size choices are remembered.

### 3. 自定义名称与头像 / Custom Names and Avatars

在设置的“个人资料”中，可以分别修改助手名称和我的名称，并为双方直接上传头像。也可以使用 1-2 个字的头像标记或图片地址。这些设置只影响控制台内的显示，不会修改 Codex 账号资料。

In **Profile** settings, you can change the assistant and user display names and upload a separate avatar for each. You can also use a one- or two-character avatar label or an image URL. These settings affect only this console and do not change the Codex account profile.

### 4. 图片预览规则 / Image Preview Rules

![Image preview rules](./04-image-preview-rules.png)

- **单击图片 / Single click:** 在右侧辅助屏预览，不遮挡主要工作区。
- **双击图片 / Double click:** 打开底部大图预览，查看细节。
- 图片预览中的“保存图片”按钮是支持的保存方式。

- **Single click:** preview the image on the right without covering the main workspace.
- **Double click:** open the large bottom preview for detailed inspection.
- Use the explicit **Save Image** button to save generated images.

## 使用前置条件 / Requirements

- **Windows:** Windows 11, 64-bit.
- **Mac:** Apple Silicon (M1/M2/M3/M4); Intel Mac is not supported yet.
- 需要本机已安装并登录 Codex。官方订阅、有效的 OpenAI API Key，或兼容当前 Codex Responses API 的第三方 Provider 都可以；你在 Codex 里怎么配置，座舱就用哪个。
- Codex must be installed and authenticated on this computer. A ChatGPT subscription, a valid OpenAI API key, or a third-party provider compatible with the current Codex Responses API can be used; the console reuses the connection already configured in Codex.
- 当前认证或 Provider 需要能在 Codex 中正常对话，网络也需要能访问对应服务。
- The active account or provider must work in Codex, and the computer must be able to reach that provider's service.
- 控制台只读取当前认证和 Provider 状态，不提供登录、退出或切换账号，也不会代写认证文件或 Provider 配置。需要变更时，请在 Codex 本体完成。
- Authentication and provider status are read-only in the console. Sign-in, sign-out, account switching, and provider changes must be completed in Codex.

## AI 优先安装 / AI-First Installation

1. 从 [Releases](https://github.com/springwen131130-del/codex-biomechanical-console/releases) 下载自己系统对应的 Beta ZIP。
2. 核对 Release 页面提供的 SHA-256。
3. 把 ZIP 的本地路径交给 Codex，并为这次安装任务开启完全访问权限。
4. 要求 Codex 先阅读压缩包内的 `AI_READ_FIRST.txt`，再自动完成校验、安装、启动和检查。

1. Download the correct Beta ZIP for your system from [Releases](https://github.com/springwen131130-del/codex-biomechanical-console/releases).
2. Verify the SHA-256 shown on the Release page.
3. Give the local ZIP path to Codex and enable Full Access for this installation task.
4. Ask Codex to read `AI_READ_FIRST.txt` first, then verify, install, launch, and check the console automatically.

人类只需要辅助处理 Windows/macOS 安全提示、文件选择器和必须肉眼确认的画面。

Human assistance is only needed for operating-system security prompts, file pickers, and visual acceptance checks.

## 两套独立工作台 / Two Independent Workspaces

Codex Desktop 与“CODEX 生物机械控制台”的对话、模型、权限和任务状态相互独立，可以同时运行；但两边复用同一套 Codex 认证与 Provider 配置。官方订阅会共享周额度，API Key 或第三方 Provider 则按各自规则计费和限流。请避免同时修改同一项目中的同一批文件。

Codex Desktop and CODEX Biomechanical Console keep separate conversations, models, permissions, and task states, and they can run at the same time. Both reuse the same Codex authentication and provider configuration. Official subscriptions share Codex quota, while API keys and third-party providers follow their own billing and rate limits. Avoid editing the same files from both workspaces at once.

安装完成后，即使电脑重新开机，也不需要先启动 Codex Desktop。直接双击桌面的“CODEX 生物机械控制台”即可复用本机 Codex 已保存的官方订阅、API Key 或第三方 Provider 配置。Codex 仍需保留在电脑中；只有认证失效、配置被删除或更换电脑用户时，才需要回到 Codex 重新配置。

After installation, you do not need to start Codex Desktop first, even after a reboot. Open CODEX Biomechanical Console directly from the desktop; it reuses the subscription, API key, or third-party provider already configured in Codex. Keep Codex installed. Reconfigure Codex only when that authentication expires, its configuration is removed, or the computer user changes.

## Beta 安全提示 / Beta Security Notice

- Windows 当前未做商业代码签名，可能显示“未知发布者”或 SmartScreen 提示。
- Mac 当前采用 ad-hoc 签名，尚未 Apple 公证，首次启动可能需要在“隐私与安全性”中确认“仍要打开”。
- 请先核对 SHA-256，不要关闭系统安全功能。

- The Windows build is not commercially code-signed yet and may show an Unknown Publisher or SmartScreen warning.
- The Mac build uses ad-hoc signing and is not Apple-notarized yet. First launch may require **Open Anyway** in Privacy & Security.
- Verify the SHA-256 first. Do not disable operating-system security features.

## 下载 / Download

请只从本仓库的 [Releases](https://github.com/springwen131130-del/codex-biomechanical-console/releases) 页面下载公开体验包。

Download public test builds only from this repository's [Releases](https://github.com/springwen131130-del/codex-biomechanical-console/releases) page.
