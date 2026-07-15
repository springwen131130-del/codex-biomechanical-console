# CODEX 生物机械控制台 / CODEX Biomechanical Console

一款可独立启动的第三方 Codex 生物机械控制台。安装完成后，不需要预先打开 Codex Desktop，可直接从桌面入口进入。

An independently launched third-party console for Codex. After installation, you can open it directly from the desktop without starting Codex Desktop first.

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
- Codex is installed and has been logged into once on this computer.
- The OpenAI/Codex account can chat normally and has available weekly Codex quota.
- The network can access OpenAI/Codex services.

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

Codex Desktop 与“CODEX 生物机械控制台”的对话、模型、权限和任务状态相互独立，可以同时运行；但两边使用同一个账号和同一份周额度。请避免同时修改同一项目中的同一批文件。

Codex Desktop and CODEX Biomechanical Console keep separate conversations, models, permissions, and task states, and they can run at the same time. They share the same account and weekly quota. Avoid editing the same files from both workspaces at once.

安装完成后，即使电脑重新开机，也不需要先启动 Codex Desktop。直接双击桌面的“CODEX 生物机械控制台”即可复用本机已保存的 Codex 登录状态。Codex 仍需保留在电脑中；只有登录失效、账号退出或更换电脑用户时才需要重新登录。

After installation, you do not need to start Codex Desktop first, even after a reboot. Open CODEX Biomechanical Console directly from the desktop; it reuses the Codex login already saved on the computer. Keep Codex installed. Sign in again only when the saved session expires, the account is logged out, or the computer user changes.

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
