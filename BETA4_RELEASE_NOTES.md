# CODEX 生物机械控制台 Beta 4

## 新增功能

1. **开放可替换外观系统**
   - 外壳主题与中央藏品可以独立替换、组合和导入。
   - 附带 Creator Kit、制作 Skill、安全区模板和提示词，可以让 Codex 帮你制作自己的主题。

2. **自定义 Provider 与多模型切换**
   - 支持填写第三方 Base URL、API Key 和多个模型 ID。
   - 配置后的模型可以在控制台顶部快速切换。

3. **Windows 云端中文语音识别**
   - 支持 `SenseVoiceSmall` 和 `TeleSpeechASR`。
   - 语音先转换为可编辑文字，确认后再发送。

4. **更完整的对话管理**
   - 对话分为置顶、普通、归档、导入本机对话四类。
   - 支持接管原对话、复制独立对话及永久删除复制副本。

5. **长对话提醒**
   - 对话达到 50 MiB 开始提醒，100 MiB 加强警示。
   - 可以一键新建对话继续，原历史不会删除。

## 修复与优化

- 优化归档、置顶、导入和复制对话的稳定性。
- 切换自定义 Provider 不再影响 Codex 本体对话列表。
- 优化第三方模型回复显示和模型切换体验。
- 优化大对话复制、删除和进度反馈。
- 优化模型菜单、配置面板滚动和文字显示。
- 修复二级屏闪烁。
- 覆盖安装时继续保留对话、头像、语言和本机配置。

## 下载

| 平台 | 文件 | SHA-256 |
| --- | --- | --- |
| Windows 普通安装 | `CODEX-Biomechanical-Console-Windows-Beta4-Setup-fb81c82.exe` | `745E4130B7F0312F0272F1E7CF4513253D20591EA459081AFEC875243518E645` |
| Windows 免安装 / 恢复 | `CODEX-Biomechanical-Console-Windows-Beta4-fb81c82.zip` | `D9DF2575F081F7C49733C62332080E001C4D7DAE356D4D8ACC41A647C44F0259` |
| Apple Silicon Mac | `CODEX-Biomechanical-Console-Mac-Beta4-ad60e58.tar.gz` | `8FBABCD01E81EB824A5C788C8B4258CFC596D1D4DAD3386FB1EFC9549BA2D92F` |

## 使用提示

- 使用前需要本机已安装并可正常使用 Codex。
- Windows 安装包尚未商业代码签名。
- Mac 版本仅支持 Apple Silicon，尚未 Apple 公证。
- 自定义 Provider 和 Windows 云端语音识别仍属于实验功能。
- Mac 自定义 Provider、云端语音和 TTS 当前不可用。
