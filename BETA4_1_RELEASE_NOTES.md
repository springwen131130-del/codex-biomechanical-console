# CODEX 生物机械控制台 Beta 4.1

这是一个 **Windows Provider / 对话隔离热修复版**。

## 修复内容

- 启用自定义 Provider 后，不再改写 Codex 本体当前 Provider。
- 控制台自己的自定义模型继续由控制台管理和调用。
- “导入本机 Codex 对话”始终读取完整本机对话列表，不再被控制台当前 Provider 过滤。
- 修复了切换回官方连接后，本体旧对话才重新出现的问题。

## 安装

- 普通用户下载 Setup EXE，直接覆盖安装即可，不要先卸载旧版。
- 免安装或恢复场景下载 ZIP。
- 更新不会主动删除控制台已有的会话映射、头像、语言和本机设置。

## 平台范围

Beta 4.1 只发布新的 Windows 资产。Apple Silicon Mac 的自定义 Provider 原本就未启用，因此继续使用已经过真机验收的 Beta 4 Mac 包。

## 安全与验收

- 源代码提交：`fb81c82`
- 自动化测试：1029 项通过，0 失败。
- 受保护核心会话与 DPAPI 凭据 smoke 通过。
- 发布扫描：内部语义、运行状态数据、VCS/CI、凭据、开发者身份五类命中均为 0。
- Windows 安装包尚未商业代码签名。
- 核心运行系统闭源；发布包开放的是经过校验的数据型外壳、藏品和 Creator Kit。

## SHA-256

```text
745E4130B7F0312F0272F1E7CF4513253D20591EA459081AFEC875243518E645  CODEX-Biomechanical-Console-Windows-Beta4.1-Setup-fb81c82.exe
D9DF2575F081F7C49733C62332080E001C4D7DAE356D4D8ACC41A647C44F0259  CODEX-Biomechanical-Console-Windows-Beta4.1-fb81c82.zip
```
