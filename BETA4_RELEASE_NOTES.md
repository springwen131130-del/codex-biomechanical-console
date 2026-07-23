# CODEX 生物机械控制台 Beta 4

Beta 4 把这套产品从“可运行的 Codex 外壳”继续推进成真正可长期使用、也能让用户创作外观的沉浸式 Agent 控制台。

## 本次重点

- **对话列表恢复为真正的四分类**：置顶、普通、归档、导入本机 Codex 对话各自独立显示；修复归档/置顶延迟、状态错乱、新对话消失与复制对话删除体验。
- **大对话人性化提示**：历史达到 50 MiB 时提醒，100 MiB 时提高警示，但不删除原记录，用户可以一键新建对话继续。
- **模型配置入口**：Windows 可使用官方 Codex，或填写用户自己确认兼容 Codex 的自定义 Provider；支持添加多个模型 ID 并在控制台切换。该能力仍是实验功能，控制台不替任何中转站认证兼容性。
- **Provider 与对话隔离修复**：自定义 Provider 只作用于控制台自己的运行，不再改写 Codex 本体当前 Provider；“导入本机 Codex 对话”始终读取完整本机对话列表。
- **语音识别实验链路**：Windows 云端 ASR 支持 `SenseVoiceSmall` 与 `TeleSpeechASR`，识别文字先保持可编辑、不会自动发送。macOS 云端语音与 TTS 尚未开放。
- **开放外观创作层**：外壳主题与中央藏品可以自由组合、导入和继续创作；Creator Kit 内含 Appearance V1 规范、安全区模板、提示词和可交给 Codex 读取的制作 Skill。
- **核心边界收紧**：Bridge、会话、事件、权限、Provider 凭据与交互骨架封装在受保护运行核心中，发布包不再散落这些核心源码。

## 下载选择

- Windows 普通用户：`CODEX-Biomechanical-Console-Windows-Beta4-Setup-fb81c82.exe`
- Windows 免安装/故障恢复：`CODEX-Biomechanical-Console-Windows-Beta4-fb81c82.zip`
- Apple Silicon Mac：`CODEX-Biomechanical-Console-Mac-Beta4-ad60e58.tar.gz`
- 下载后请用 `SHA256SUMS.txt` 核对文件。

Windows 资产由核心提交 `fb81c82` 构建，完成 1029 项自动化测试、真实启动、升级保留与发布内容扫描。Apple Silicon Mac 保留由提交 `ad60e58` 构建并完成真机验收的 Beta 4 资产；Mac 自定义 Provider 尚未开放，因此不受本次 Windows Provider 隔离修复影响。

## 安全与已知限制

- 核心运行系统闭源；发布包开放的是经过校验的数据型外壳、藏品和 Creator Kit。
- 发布扫描中，内部语义、运行状态数据、VCS/CI、凭据、开发者身份五类命中均为 0。
- Windows 安装包尚未商业代码签名。
- macOS 仅验证 Apple Silicon；当前只有 ad-hoc 临时签名，尚未 Apple 公证，不支持 Intel Mac。
- Windows 自定义 Provider 与云端 ASR 为实验功能；不同服务商和模型是否可用，以用户购买服务的真实兼容性为准。
- macOS 自定义 Provider、macOS 云端 ASR、TTS、多智能体和 Agent 角色包尚未开放。

完整安装、隐私和创作边界请阅读发布包内 `docs` 与 `creator-kit`。

---

Beta 4 adds explicit conversation categories, humane long-history warnings, an experimental Windows Custom Provider/model switcher, cloud ASR, Appearance V1, and a Codex-readable Creator Kit. The refreshed Windows assets are built from `fb81c82` and keep Custom Provider state isolated from the native Codex provider and conversation list. The accepted Apple Silicon asset remains on `ad60e58` because Custom Provider is not enabled on macOS. Windows remains unsigned; macOS is ad-hoc signed and not notarized.
