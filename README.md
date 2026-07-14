# CODEX 生物机械控制台

一款可独立启动的 Codex 生物机械控制台。安装完成后，不需要预先打开 Codex Desktop，可直接从桌面入口进入。

> 本项目是独立第三方体验项目，不修改 Codex Desktop，也不公开核心接入源码。

## 使用前置条件

- Windows：Windows 11，64 位。
- Mac：Apple Silicon（M1/M2/M3/M4），暂不支持 Intel Mac。
- 电脑已安装 Codex，并已登录可正常对话的 OpenAI/Codex 账号。
- 账号具有可用的 Codex 周额度，网络能够访问 Codex 服务。

## AI 优先安装

1. 从 [Releases](../../releases) 下载自己系统对应的 Beta ZIP。
2. 核对 Release 页面提供的 SHA-256。
3. 把 ZIP 的本地路径交给 Codex，并为这次安装任务开启完全访问权限。
4. 要求 Codex 先阅读压缩包内的 `AI_READ_FIRST.txt`，再自动完成校验、安装、启动和检查。

人类只需要辅助处理 Windows/macOS 安全提示、文件选择器和必须肉眼确认的画面。

## 两套工作台

Codex Desktop 与“CODEX 生物机械控制台”的对话、模型、权限和任务状态相互独立，可以同时运行；但两边使用同一个账号和同一份周额度。请避免同时修改同一项目中的同一批文件。

## Beta 安全提示

- Windows 当前未做商业代码签名，可能显示“未知发布者”或 SmartScreen 提示。
- Mac 当前采用 ad-hoc 签名，尚未 Apple 公证，首次启动可能需要在“隐私与安全性”中确认“仍要打开”。
- 请先核对 SHA-256，不要关闭系统安全功能。

## 下载

请只从本仓库的 [Releases](../../releases) 页面下载公开体验包。