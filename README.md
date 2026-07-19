# CODEX 生物机械控制台 / CODEX Biomechanical Console

**CODEX 控制台连接真实 Codex，把对话、运行、等待和完成状态重新组织成一台本地 AI 控制台。**

未来的工作不该无聊。让每一次对话、运行、等待和完成，都像在操纵一台真正的生物机械装置。

在视觉设计上，它致敬我最爱的《暗黑破坏神》，也致敬 H.R. 吉格笔下诡异、冷峻而充满生命感的生物机械美学。

**这不是游戏，也不是概念图。**

使用前需要本机已安装并登录 Codex。安装控制台后，不需要提前手动打开 Codex Desktop；直接从桌面入口启动即可，控制台会复用本机 Codex 已保存的登录状态。

**CODEX Console connects to real Codex and reorganizes conversations, runs, waiting states, and completions into a local AI control console.**

The future of work should not feel boring. Every conversation, run, wait, and completion should feel like operating a real biomechanical machine.

Its visual design is a personal tribute to the dark fantasy of *Diablo* and the strange, cold, living biomechanical art of H. R. Giger.

**This is not a game or a concept render.**

Codex must be installed and authenticated on this computer before use. After installation, you do not need to start Codex Desktop manually first; open the console from the desktop, and it will reuse the login state already saved by Codex.

> 本项目不修改 Codex Desktop，也不公开核心接入源码。
>
> This project does not modify Codex Desktop and does not publish its private integration source code.

## 界面一览 / Console Overview

![CODEX Biomechanical Console overview](./01-console-overview.png)

- **左侧 / Left:** Codex 对话与输入区 / Codex chat and composer.
- **中间 / Center:** 动态主题藏品区 / animated themed collection.
- **右侧 / Right:** 设置、预览和辅助信息屏 / settings, previews, and auxiliary information.
- **底部 / Bottom:** 新对话、搜索、插件、电脑控制、项目和预览快捷入口 / shortcuts for chat, search, plugins, Computer Use, projects, and preview.

## Beta 3 新增功能 / What's New in Beta 3

- **导入本机 Codex 对话：** 可选择“接管同一条对话”继续原记录，或“复制为独立新对话”创建独立分叉；不会自动导入全部历史。
- **电脑控制权限：** 新增“每步询问 / 自动审查 / 完全控制”三档，并与文件、命令访问权限分开管理。
- **语音输入：** 输入栏新增麦克风按钮，可把语音转换为可编辑文字，确认后再发送。
- **本地项目实时预览：** 当前任务启动本地服务后，可在控制台中直接打开、刷新、滚动和交互，也可外部打开或保存截图。
- **个人资料：** 可分别修改用户与助手名称并上传头像。
- **语言入口：** 顶部“语言”和“设置 → 语言”进入同一个中英文设置页，选择会被记住。
- **Provider 状态：** 只读显示 Codex 当前 Provider，不修改登录、认证或 Provider 配置。
- **体验修复：** 优化暂停后的消息显示、完成状态收敛、头像裁切、预览面板拉伸和滚动等细节。

- **Import local Codex conversations:** resume the same native conversation or fork it as an independent chat; full history is never imported automatically.
- **Computer Use permissions:** choose Ask Each Step, Auto Review, or Full Control separately from file and command access.
- **Voice input:** convert speech into editable text from the composer microphone, then review it before sending.
- **Interactive local project preview:** open, refresh, scroll, and use a local service started by the current task, with external-open and screenshot fallbacks.
- **Profile:** set separate user and assistant names and upload avatars.
- **Language entry:** the top Language control and Settings → Language open the same persistent Chinese/English page.
- **Provider status:** display the current Codex provider read-only without changing authentication or provider configuration.
- **UX fixes:** improved interrupted-turn display, completion convergence, avatar cropping, preview resizing, and scrolling.

## 常用交互 / Essential Controls

### 1. 主题藏品切换 / Theme Collection Switch

![Theme and collection switch](./02-skin-and-collection-switch.png)

点击中下方的核心按钮，会循环切换中心动态藏品以及与它配套的整套主题外壳。

Click the lower-center core control to cycle both the animated center collection and its matching shell theme.

### 2. 设置是两步操作 / Settings Use a Two-Step Flow

![Settings two-step flow](./03-settings-two-step.png)

先点击左下发光设置节点，再在右侧辅助屏选择语言、输入字号、模型、推理强度等选项。顶部“语言”也会直接打开同一个语言设置页。语言和字号选择会被记住。

First click the glowing Settings node in the lower-left corner, then choose language, input size, model, reasoning effort, and other options on the right auxiliary screen. The top Language control opens the same language settings page. Language and font-size choices are remembered.

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
- 当前公开 Beta 3 需要本机已安装 Codex，并已通过官方 ChatGPT 账号完成认证且能正常对话。
- The current public Beta 3 requires Codex to be installed and working with official ChatGPT account authentication.
- 有效 OpenAI API Key 与兼容当前 Codex Responses API 的第三方 Provider 仍在独立验收，暂不宣称 Beta 3 已兼容。
- Valid OpenAI API keys and third-party providers compatible with the current Codex Responses API remain under separate acceptance testing and are not currently claimed as Beta 3 compatible.
- 当前 Beta 3 使用的官方 ChatGPT 账号需要能在 Codex 中正常对话，网络也需要能访问 Codex 服务。
- The official ChatGPT account used by Beta 3 must work in Codex, and the computer must be able to reach Codex services.
- 控制台不提供登录、退出或切换账号；需要变更时，请在 Codex 本体完成。Provider 状态只读显示，不会代写认证文件或 Provider 配置。
- The console does not provide sign-in, sign-out, or account switching. Complete those actions in Codex. Authentication and provider status are read-only; the console will not rewrite authentication or provider configuration files.

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

Codex Desktop 与“CODEX 生物机械控制台”的对话、模型、权限和任务状态默认相互独立，可以同时运行；当前 Beta 3 复用同一个官方 ChatGPT 账号并共享周额度。API Key 与第三方 Provider 仍在独立验收。请避免同时修改同一项目中的同一批文件。

Codex Desktop and CODEX Biomechanical Console keep separate conversations, models, permissions, and task states by default, and they can run at the same time. The current Beta 3 reuses the same official ChatGPT account and quota. API-key and third-party-provider support remains under separate acceptance testing. Avoid editing the same files from both workspaces at once.

在“导入本机 Codex 对话”中选择“接管同一条对话”后，控制台会继续写入同一条原生对话记录；Desktop/CLI 需要重新载入才能看到新增内容，请勿两端同时操作。选择“复制为独立新对话”会创建新的对话记录，但不会复制项目文件，两条对话默认共用原工作区，请勿同时修改。

When you choose **Use Same Conversation**, the console continues the same native conversation record. Reload Desktop/CLI to see new turns, and do not use both clients on that conversation at the same time. **Copy as Independent Chat** creates a new conversation record but does not copy project files; both conversations use the original workspace by default, so do not edit it from both at once.

安装完成后，即使电脑重新开机，也不需要先启动 Codex Desktop。直接双击桌面的“CODEX 生物机械控制台”即可复用本机 Codex 已保存的官方 ChatGPT 账号认证。Codex 仍需保留在电脑中；只有认证失效、账号退出或更换电脑用户时，才需要回到 Codex 重新认证。

After installation, you do not need to start Codex Desktop first, even after a reboot. Open CODEX Biomechanical Console directly from the desktop; it reuses the official ChatGPT account authentication already saved by Codex. Keep Codex installed. Reauthenticate in Codex only when that authentication expires, the account is signed out, or the computer user changes.

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
