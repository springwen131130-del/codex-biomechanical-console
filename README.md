# CODEX 生物机械控制台

## 别人给 Codex 换脸，我们给它造身体。

### Others reskin Codex. We give it a body.

**真实工作，真实回应；外壳与藏品，由每个人创造。**

同一颗 Codex 心脏，一副由我们设计的沉浸式交互骨架，无数由你创造、组合和分享的未来世界。

[立即下载 Beta 4](https://github.com/springwen131130-del/codex-biomechanical-console/releases/tag/v0.1.0-beta.4) · Windows 与 Apple Silicon Mac 都在同一个 Release，使用官方典藏款，或让你自己的 Codex 帮你造一套。

连接真实 Codex，把对话、运行、审批、等待、完成和项目预览，重新组织成一台可以每天使用的本地沉浸式 AI 控制台。

**不是游戏概念图，不是覆盖在原版界面上的壁纸，也不是只有颜色变化的网页主题。**

- 真正调用本机 Codex，会写文件、执行命令并持续原生会话；
- 三舱式控制台把对话、动态藏品、设置和项目预览放进同一套交互骨架；
- 长对话在变卡前主动提醒，复制副本可单独释放磁盘空间；
- 外壳与中央藏品可以独立更换，也能让自己的 Codex 帮你制作新主题；
- 核心运行系统闭源，开放的是经过校验的数据型外观创作层。

> 本 README 对应重新发布的 **Beta 4**。公开可见版本、下载资产与 SHA-256 始终以 Releases 页面实际列出的内容为准。

![CODEX 生物机械控制台总览](./01-console-overview.png)

## 它到底多做了什么

### 1. 真正工作的沉浸式控制台

左舱负责对话、文件与输入，中舱负责主题藏品和运行氛围，右舱负责设置、会话列表、状态与辅助预览；底部保留新对话、搜索、插件、电脑控制、项目和实时预览入口。

它不修改 Codex Desktop，也不需要每次先打开 Desktop 窗口。控制台会连接本机 Codex 的真实运行能力，自己的对话空间可以与 Desktop 同时存在。

### 2. 对话不是堆在一起，而是真正分类

Beta 4 把列表改为四个互斥入口：**置顶、普通、归档、导入本机 Codex 对话**。点哪一栏，就只显示哪一栏。

导入时可以：

- **接管同一条对话：** 继续原生记录；
- **复制为独立新对话：** 创建可单独工作的副本；
- **永久删除复制副本：** 只清理副本，原对话和项目文件不受影响；
- **从控制台移除：** 只解除绑定，不删除磁盘记录。

大对话复制会显示处理阶段和已耗时。Codex 没有提供真实字节进度时，控制台不会伪造百分比。

### 3. 比原生工作流多一步的人性化预警

单条会话历史达到 **50 MiB** 时显示“历史较重”，达到 **100 MiB** 时升级为“历史临界”。提醒会说明图片和长历史可能拖慢后续回复，并提供“新建会话”入口。

提醒不会自动删除、归档、切换或中断当前任务；原历史始终保留。

### 4. 本地项目就在控制台里看

当前任务启动本地服务后，可以直接在控制台中打开、刷新、滚动和交互，也可以在系统浏览器打开或保存截图。项目预览只接受本机回环地址。

### 5. 电脑控制与文件权限分开

Computer Use 提供“每步询问 / 自动审查 / 完全控制”三档，和文件、命令访问权限分别管理。界面只显示真实能力；目标智能体不支持的功能不能用一个假按钮代替。

### 6. 先是一套作品，再变成创作者生态

Beta 4 Appearance V1 把**外壳主题**和**中央藏品**拆成两个独立选择器。用户可以使用官方典藏款，也可以导入自己制作的安全外观包。

![外壳与中央藏品切换](./02-skin-and-collection-switch.png)

## 心脏、骨架、皮相、角色

```text
第一层：心脏  →  真实 Codex Runtime，闭源运行核心
第二层：骨架  →  官方设计的屏幕结构、功能布局与交互母版
第三层：皮相  →  开放的外壳、材质、背景、动效与中央藏品
第四层：角色  →  Agent 形象、身份、音色与表达风格（规划中）
```

**功能由我们维护，主题由每个人创造。**

Beta 4 已开放第三层中的外壳与藏品；布局编辑器和可安装 Agent 角色包尚未实现。头像、名称设置不等于角色包系统。

外观包只允许声明、参数和经过校验的本地数据与媒体。它不能携带 JavaScript、命令脚本、远程代码、Provider、接口或密钥，也不能改变权限、伪造运行状态或脱离控制台核心独立运行。

## Creator Kit：让自己的 Codex 帮你造一套

Beta 4 发布包附带外观创作工具包，包含：

- 外壳与中央藏品安全区模板；
- 赛博朋克、军事、国风机关、鲜花宫殿和深海主题提示词范本；
- 可直接复制的外壳包、藏品包示例；
- 本地校验与 SHA-256 清单工具；
- 导入、恢复默认和截图分享说明。

最短流程：告诉 Codex 你想要的世界 → 选择模板 → 生成媒体 → 本地校验 → 导入控制台 → 晒出自己的座舱。

Creator Kit 只用于制作可替换外壳与藏品，不会改变控制台功能。

## Beta 4 实验入口：模型配置

Beta 4 把“模型配置”放到明面入口，并分成 **智能模型、语音识别、语音合成** 三个功能区。智能模型区只显示 **官方 Codex + 自定义 Provider**，不与任何单一中转站绑定。

自定义 Provider 的流程只有两步：

1. 填写名称、Base URL、API Key，并用“+ 添加模型”录入一个或多个准确模型 ID；模型 ID 由用户从自己购买服务的网站复制。
2. 点击**保存并应用**；Key 只提交给本机核心，Windows 使用当前用户的 **DPAPI** 加密保存，不写入浏览器 `localStorage`、普通配置或日志。

保存后的模型会进入控制台模型下拉框，用户可以随时切换。控制台不会替服务商读取或维护模型目录，只检查本地格式、事务写入和配置回读，且**不认证任何中转站兼容性**。请使用自己已经确认兼容 Codex 的服务；配置失败会回滚。恢复官方连接时，已经保存的 Key 会保留，之后可以直接重新应用。

**LLM 与 ASR 凭据彼此独立**，不会跨功能自动共用；TTS 当前没有凭据配置。

### 独立合作入口

界面中的**购买 API 额度**是独立合作链接，官网地址由核心返回固定 HTTPS 目标，客户端不接受页面随意指定跳转地址。它不会自动填写或改变自定义 Provider，也不会把产品绑定到点力 Token。

用户是否能在自身网络环境使用，取决于服务本身和实际连通性；控制台不替服务商保证兼容。

### 语音服务不是同一件事

Windows 云端语音识别支持 `SenseVoiceSmall` 与 `TeleSpeechASR` 两个模型。

合作方接口接受 MP3/WAV；Windows 客户端只录制并上传 **16 kHz 单声道 WAV**。只有用户明确开始并结束云端录音后，这一段录音才会提交给第三方；返回文字保持可编辑，识别结果不会自动发送。

Windows 云端语音识别按 **Beta 4 实验功能**提供；macOS 云端语音与语音合成 / TTS 当前不可用。

## 常用交互

### 设置采用两步操作

![设置两步操作](./03-settings-two-step.png)

先点击左下发光设置节点，再在右侧辅助屏选择语言、输入字号、模型、智能等级、外观与连接设置。顶部“语言”会打开同一页，语言和字号会被记住。

### 图片单击与双击各有用途

![图片预览规则](./04-image-preview-rules.png)

- 单击：在右侧辅助屏预览，不挡住主工作区；
- 双击：在底部打开大图检查细节；
- 保存：使用预览里的明确“保存图片”按钮。

### 用户与 Agent 可以有各自身份

设置中可分别修改双方名称和头像，只影响控制台内显示，不会修改 Codex 账号资料。

## 当前版本边界

### 已公开 Beta 3

- 需要本机已安装 Codex，并完成可用的官方 ChatGPT 账号认证；
- Windows 11 64 位；macOS 仅 Apple Silicon；
- Provider 在 Beta 3 中仍为只读状态；
- Windows 未商业代码签名；Mac 未 Apple 公证。

### Beta 4 发布版

- 四分类会话列表、复制进度、复制副本删除和长历史提醒；
- Appearance V1 与 Creator Kit；
- Windows 模型配置与云端 ASR 实验入口；
- Windows 11 x64 与 Apple Silicon 安装包。

Provider Hub 在 macOS 上必须先完成系统 Keychain 凭据实现与真机验证，不能把 Windows DPAPI 方案直接当成跨平台完成。

### Beta 4 Provider 与对话优化

- 切换自定义 Provider 不再影响 Codex 本体对话列表；
- 优化本机对话导入和模型切换体验。

## AI 优先安装

1. 从 [Releases](https://github.com/springwen131130-del/codex-biomechanical-console/releases) 下载与系统对应、实际公开的 Beta 包。
2. 核对 Release 页面提供的 SHA-256。
3. 把下载文件的本地路径交给 Codex，为安装任务开启所需文件与命令权限。
4. 让 Codex 先阅读压缩包内 `docs/AI_READ_THIS_FIRST.md`，再校验、安装、启动和检查。

升级时直接覆盖安装，不要先卸载旧版；会话映射、头像、语言与本机设置应继续保留。

## 两套工作台如何相处

Codex Desktop 与本控制台默认拥有各自的对话、模型、权限和任务状态，可以同时运行，但不要同时修改同一个项目中的同一批文件。

“接管同一条对话”会继续写原记录，Desktop/CLI 重新载入后才能看到新增内容，请勿两端同时操作同一会话。“复制为独立新对话”只复制会话记录，不复制项目文件；需要并行开发时，请为副本准备独立目录或 Git worktree。

## 安全与隐私

- 本项目是第三方沉浸式 Codex 客户端，不是 OpenAI 官方产品；
- 官方账号认证只读；控制台不提供登录、退出或切换账号；
- 开放的是可替换外壳、藏品与创作工具，不是底层核心源码；
- 不把 API Key 写进主题包、前端存储、日志或 Git；
- 不从来源和哈希不明的地址安装；

## Download / 下载

只从本仓库的 [Beta 4 Release](https://github.com/springwen131130-del/codex-biomechanical-console/releases/tag/v0.1.0-beta.4) 下载，并按下面的 SHA-256 核对文件。重新发布的 Beta 4 Windows 资产由核心提交 `fb81c82` 构建；Apple Silicon Mac 保留核心提交 `ad60e58` 的已验收资产。两者都经过真实启动或对应平台验收与发布内容扫描。Windows 尚未商业代码签名，Mac 只有 ad-hoc 临时签名且尚未 Apple 公证。

| 平台 | 文件 | SHA-256 |
| --- | --- | --- |
| Windows 普通安装 | [`CODEX-Biomechanical-Console-Windows-Beta4-Setup-fb81c82.exe`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/CODEX-Biomechanical-Console-Windows-Beta4-Setup-fb81c82.exe) | `745E4130B7F0312F0272F1E7CF4513253D20591EA459081AFEC875243518E645` |
| Windows 免安装 / 恢复 | [`CODEX-Biomechanical-Console-Windows-Beta4-fb81c82.zip`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/CODEX-Biomechanical-Console-Windows-Beta4-fb81c82.zip) | `D9DF2575F081F7C49733C62332080E001C4D7DAE356D4D8ACC41A647C44F0259` |
| Apple Silicon Mac | [`CODEX-Biomechanical-Console-Mac-Beta4-ad60e58.tar.gz`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/CODEX-Biomechanical-Console-Mac-Beta4-ad60e58.tar.gz) | `8FBABCD01E81EB824A5C788C8B4258CFC596D1D4DAD3386FB1EFC9549BA2D92F` |
| 校验清单 | [`SHA256SUMS.txt`](https://github.com/springwen131130-del/codex-biomechanical-console/releases/download/v0.1.0-beta.4/SHA256SUMS.txt) | — |

如果你也觉得 AI 工具不该只剩一块白色聊天框：

- 给仓库一个 Star，方便回来查看新版本；
- 用 Creator Kit 做出自己的外壳或藏品；
- 截图分享你的 Codex 座舱，让下一个世界从你的版本继续长出来。

## English summary

**Give Codex more than a new face—give it a futuristic body that works and responds.**

CODEX Biomechanical Console is a third-party local client connected to real Codex capabilities. It adds an immersive three-bay interaction chassis, explicit conversation management, proactive 50/100 MiB history notices, interactive local project preview, validated data-only appearance packs, and a Creator Kit.

Public downloads remain whatever is actually listed on the Releases page. The refreshed Beta 4 Windows package keeps Custom Provider selection inside the console and restores the complete local Codex conversation list. The accepted Apple Silicon package remains on `ad60e58` because Custom Provider is not enabled there. The Windows-only experimental Provider Hub shows Official Codex and one neutral Custom Provider configuration. Users enter a name, Base URL, API key, and one or more exact model IDs; saved models become available in the console model selector. The console validates local configuration but does not fetch a provider catalogue or certify relay compatibility. Buy API Credit is a separate partner link. LLM and ASR credentials remain separate, and restoring Official Codex keeps saved keys. Dianli ASR passed six isolated human-recording requests across both advertised models; the Windows 16 kHz mono-WAV path ships only as an experimental feature, and results remain editable and are never auto-sent. macOS cloud speech and TTS are unavailable. Windows is not commercially code-signed; the Apple Silicon app passed real-device launch checks with an ad-hoc signature but is not Apple-notarized.
