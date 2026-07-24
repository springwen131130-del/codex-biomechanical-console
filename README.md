# CODEX 氛围主题智能体控制台

## 它不仅仅是一套主题外观，也不仅仅是一个聊天界面。

这是一台连接真实 Codex、可以每天打开并沉浸其中工作的 **AI 智能体控制台**。

Codex 会写代码、执行命令、调用工具并持续处理任务。这里把真实的运行、等待、工具活动、文件变化、审批和结果，重新组织进一个看得见、可以介入的工作空间。

[立即下载 Beta 4](https://github.com/springwen131130-del/codex-biomechanical-console/releases/tag/v0.1.0-beta.4) · Windows 11 x64 / Apple Silicon Mac

![CODEX 氛围主题智能体控制台总览](./01-console-overview.png)

## 为什么它用起来不再只是聊天？

因为这里把“和 AI 一起工作”的感觉，从**发消息、等回复**，变成了**像在操作一台真正工作的强大机器**。

你不必只盯着最后一条回答。智能体是在运行、等待、调用工具，还是已经完成；它产生了哪些文件变化和执行结果；什么时候需要你审批或介入——这些工作线索都被放回同一个控制台里。

> 这不是一张覆盖在 Codex 上面的壁纸，而是一个连接本机 Codex 真实运行能力的第三方工作台。

## 你会实际看见什么？

- **任务正在发生什么：** 运行、等待、工具活动、错误和完成状态会进入界面，而不是只剩一个转圈提示。
- **智能体留下了什么：** 文件改动、工具输出、事件摘要、图片和本地项目结果可以继续查看。
- **什么时候需要你：** 审批、停止和 Computer Use 控制都有明确入口，不需要靠猜。
- **长期工作放在哪里：** 对话可以导入、接管、复制、置顶、归档或从控制台移除。
- **项目最后长什么样：** 本地服务启动后，可以直接在控制台里预览、刷新、滚动、交互和截图。

界面不会伪造模型隐藏思考，也不会编造固定步骤或完成百分比；没有真实上游事件时，就不假装知道。

## 把长期任务当成工作，而不是消息堆

Beta 4 把对话分成四个互斥入口：**置顶、普通、归档、导入本机 Codex 对话**。点哪一栏，就只看哪一栏。

导入本机对话时可以选择：

- **接管同一条对话：** 继续写入原生记录；
- **复制为独立新对话：** 保留原对话，创建可单独工作的副本；
- **永久删除复制副本：** 释放副本占用的空间，不影响原对话和项目文件；
- **从控制台移除：** 只解除控制台绑定，不删除磁盘记录。

大对话复制会显示真实处理阶段和已耗时。单条历史达到 **50 MiB** 时出现“历史较重”提醒，达到 **100 MiB** 时升级为“历史临界”，并提供新建对话入口；提醒不会擅自删除、归档或中断当前任务。

## 一台可以每天打开的工作台

三舱式交互骨架把输入与对话、动态工作区、状态与辅助预览放进同一个空间；底部保留新对话、搜索、插件、电脑控制、项目和实时预览入口。

它不修改 Codex Desktop，也不要求每次先打开 Desktop 窗口。控制台连接本机 Codex 的运行能力，拥有自己的任务状态和工作界面，也可以与 Desktop 同时存在。

### 本地项目直接看

当前任务启动本地服务后，可以在控制台中打开、刷新、滚动和交互，也可以在系统浏览器打开或保存截图。项目预览只接受本机回环地址。

### 权限与电脑控制分开

Computer Use 提供“每步询问 / 自动审查 / 完全控制”三档，并与文件、命令访问权限分开管理。界面只展示真实可用能力，不用假按钮冒充尚未接入的功能。

## 让这台机器长成你喜欢的样子

真实 Codex 能力是心脏，交互控制台是骨架；外框、中央藏品和未来的 Agent 角色，则是可以继续生长的创作层。

```text
第一层：心脏  →  真实 Codex Runtime，闭源运行核心
第二层：骨架  →  官方设计的屏幕结构、功能布局与交互母版
第三层：皮相  →  开放的外框、材质、背景、动效与中央藏品
第四层：角色  →  Agent 形象、身份、音色与表达风格（规划中）
```

Beta 4 已经开放第三层中的外框和藏品。两者可以独立选择，也可以通过中央实体“皮肤切换”按钮使用官方配对组合。

![外框与中央藏品切换](./02-skin-and-collection-switch.png)

### Creator Kit：让自己的 Codex 帮你造一套

Beta 4 发布包附带创作工具包：

- 外框与中央藏品安全区模板；
- 赛博朋克、军事、国风机关、鲜花宫殿和深海主题提示词；
- 可直接复制的外观包示例；
- 本地校验和 SHA-256 清单工具；
- 导入、恢复默认和截图分享说明。

最短流程：告诉 Codex 你想要的世界 → 选择模板 → 生成媒体 → 本地校验 → 导入控制台。

外观包只包含经过校验的数据与媒体，不能携带 JavaScript、命令脚本、远程代码、Provider、接口或密钥，也不能修改权限和真实工具行为。Beta 4 尚未提供可安装 Agent 角色包。

## 三步开始使用 Beta 4

1. 从 [Beta 4 Release](https://github.com/springwen131130-del/codex-biomechanical-console/releases/tag/v0.1.0-beta.4) 下载对应平台版本。
2. 核对 Release 页面中的 SHA-256，然后直接安装或覆盖旧版本。
3. 启动控制台，继续使用本机已经可用的 Codex；需要时再导入本机对话。

如果你愿意让 Codex 协助安装，可以把下载文件的本地路径交给它，并让它先阅读压缩包中的 `docs/AI_READ_THIS_FIRST.md`。

## Beta 4 发布版包含什么

- 四分类对话列表、接管与复制、复制进度、副本删除和长历史提醒；
- 真实运行状态、工具状态、文件变化、事件摘要和结果预览；
- Computer Use 分级控制与独立的文件、命令权限；
- 本地项目实时预览、图片预览和截图；
- Appearance V1、四套官方外框与藏品以及 Creator Kit；
- Windows 模型配置与云端 ASR 实验入口；
- Windows 11 x64 与 Apple Silicon Mac 安装包。

> 本 README 对应已公开的 **Beta 4 发布版**。下载资产和 SHA-256 始终以 Releases 页面实际列出的内容为准。

## 实验功能与平台边界

### Windows 自定义 Provider

模型配置区显示 **官方 Codex + 自定义 Provider**，不与任何单一中转站绑定。

Windows 用户可以填写第三方服务名称、Base URL、API Key，并用“+ 添加模型”录入一个或多个准确模型 ID。点击**保存并应用**后，模型会进入控制台顶部选择器。

控制台不读取服务商的模型目录，也**不认证任何中转站兼容性**。请只填写自己已经确认兼容 Codex 的服务。Windows 使用当前用户的 DPAPI 保存凭据，不写入浏览器 `localStorage`、普通配置或日志。

切回**恢复官方连接**时，已经保存的第三方配置和 Key 会保留，方便以后重新启用。官方 Codex 账号仍由 Codex 本体管理；控制台只读取连接状态，不提供登录、退出或切换账号。

### 独立合作入口

界面中的**购买 API 额度**只是独立的合作链接，不会自动填写或改变自定义 Provider。当前链接指向点力 Token，但这不代表控制台绑定该服务，也不代表双方已经建立分成或返佣关系。

### Windows 云端语音识别

Windows 云端 ASR 实验入口支持 `SenseVoiceSmall` 与 `TeleSpeechASR`。客户端录制并上传 **16 kHz 单声道 WAV**；识别结果保持可编辑，且不会自动发送。

**LLM 与 ASR 凭据彼此独立**，不会跨功能自动共用。TTS 当前没有凭据配置。

macOS 当前不提供自定义 Provider、云端语音和 TTS；Windows Provider 与云端 ASR 也仍属于实验功能。

## 常用交互

### 设置采用两步操作

![设置两步操作](./03-settings-two-step.png)

先点击左下发光设置节点，再在右侧辅助屏选择语言、输入字号、模型、智能等级、外观与连接设置。顶部“语言”会进入同一设置区域。

### 图片单击与双击各有用途

![图片预览规则](./04-image-preview-rules.png)

- 单击：在右侧辅助屏预览；
- 双击：在底部打开大图；
- 保存：使用预览中的“保存图片”按钮。

### 用户与 Agent 可以有各自身份

设置中可以分别修改双方名称和头像，只改变控制台内显示，不修改 Codex 账号资料。

## 两套工作台如何相处

Codex Desktop 与本控制台拥有各自的任务、模型、权限和界面状态，可以同时运行，但不要让两端同时修改同一个项目中的同一批文件。

“接管同一条对话”会继续写原记录，Desktop/CLI 重新载入后才能看到新增内容。“复制为独立新对话”只复制对话记录，不复制项目文件；需要并行开发时，请准备独立目录或 Git worktree。

## 安全与安装说明

- 本项目是第三方沉浸式 Codex 控制台，不是 OpenAI 官方产品；
- 使用前需要本机已经安装并可以正常使用 Codex；
- 官方账号认证由 Codex 本体管理，控制台不代写 `auth.json`；
- 开放的是外框、藏品和创作工具，不是底层运行核心源码；
- API Key 不会写入主题包、前端存储、日志或 Git；
- Windows 安装包尚未商业代码签名；
- Mac 仅支持 Apple Silicon，使用 ad-hoc 临时签名，尚未 Apple 公证；
- 升级时直接覆盖安装，不需要先卸载旧版，本机对话映射、头像、语言和设置应继续保留。

## Download / 下载

只从本仓库的 [Beta 4 Release](https://github.com/springwen131130-del/codex-biomechanical-console/releases/tag/v0.1.0-beta.4) 下载，并按下面的 SHA-256 核对文件。当前 Windows 资产来自核心提交 `fb81c82`；Apple Silicon Mac 资产来自已验收提交 `ad60e58`。

| 平台 | 文件 | SHA-256 |
| --- | --- | --- |
| Windows 普通安装 | [`CODEX-Biomechanical-Console-Windows-Beta4-Setup-fb81c82.exe`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/CODEX-Biomechanical-Console-Windows-Beta4-Setup-fb81c82.exe) | `745E4130B7F0312F0272F1E7CF4513253D20591EA459081AFEC875243518E645` |
| Windows 免安装 / 恢复 | [`CODEX-Biomechanical-Console-Windows-Beta4-fb81c82.zip`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/CODEX-Biomechanical-Console-Windows-Beta4-fb81c82.zip) | `D9DF2575F081F7C49733C62332080E001C4D7DAE356D4D8ACC41A647C44F0259` |
| Apple Silicon Mac | [`CODEX-Biomechanical-Console-Mac-Beta4-ad60e58.tar.gz`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/CODEX-Biomechanical-Console-Mac-Beta4-ad60e58.tar.gz) | `8FBABCD01E81EB824A5C788C8B4258CFC596D1D4DAD3386FB1EFC9549BA2D92F` |
| 校验清单 | [`SHA256SUMS.txt`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/SHA256SUMS.txt) | — |

如果这就是你想每天打开的 AI 工作空间：

- 下载 Beta 4，先用一项真实任务感受完整过程；
- 用 Creator Kit 做出自己的外框或中央藏品；
- 截图分享你的控制台，让别人看到你的 AI 是怎样工作的。

## English summary

**It is not just a visual theme or another chat window. It is an AI agent control console you can open every day and actually work in, with real Codex running underneath.**

CODEX Atmosphere Theme Agent Console reorganizes real run, wait, tool, file-change, approval and result signals into an immersive workspace. It also provides explicit long-session management, local project preview, Computer Use controls, validated data-only appearance packs and a Creator Kit.

The public Beta 4 release supports Windows 11 x64 and Apple Silicon Mac. Windows Custom Provider and cloud ASR remain experimental and are not available in the accepted Mac build. Custom Provider accepts user-supplied service details and exact model IDs but does not fetch a provider catalogue or certify relay compatibility. The Buy API Credit button is a separate partner link, not an automatic provider configuration. LLM and ASR credentials remain separate. Windows is not commercially code-signed; the Apple Silicon build uses an ad-hoc signature and is not Apple-notarized.
