# TaskOnward

**换到新对话，接着做同一个任务。**

TaskOnward 帮你把当前任务现场带入新的 AI 对话，避免每次从头解释。它不是聊天记录完整备份，也不会在普通聊天时持续采集。

[免费开始](https://taskonward.5188688.xyz/start) · [Power 安装说明](docs/power-browser-assistant.md)

## 当前版本

| 版本 | 支持平台 | 状态 |
|---|---|---|
| **Power 0.8.8** | ChatGPT | **官网默认公开下载** |
| **跨平台 Power 0.4.6** | ChatGPT、Claude、Gemini | **小范围观察使用** |
| Power 0.8.7 | ChatGPT | 旧版回滚包 |

**0.4.6 暂不提供给新用户直接安装。** 原因是不同解压安装目录可能产生不同 Chrome 扩展 ID，而 WorkOS 登录回调目前只登记了既有观察安装的 ID。固定 ID 分发和全新安装登录未验收前，官网仍默认提供 0.8.8。

## 公开稳定版 Power 0.8.8

1. 下载、安装 Power 0.8.8，并使用 TaskOnward 账号登录。
2. **在 ChatGPT 中添加并连接 TaskOnward MCP**，服务器地址 `https://taskonward.5188688.xyz/mcp`，用于新 Chat 恢复；具体见[安装说明](docs/power-browser-assistant.md)。
3. 在旧 ChatGPT 对话点击 Power，等待复制交接内容。
4. 新开 ChatGPT 对话，粘贴并手动发送；确认 TaskOnward 真正取回交接后，再明确下一步。

**只靠连接 MCP 并在旧对话发送“保存任务”不能生成续聊码。** 0.8.8 必须由 Power 产生交接，并由目标 ChatGPT 的 TaskOnward MCP 读取。保存的是有界的最近任务现场，不是完整聊天归档或永久项目记忆。

## 跨平台观察版 0.4.6

供**已经授权并安装观察版**的用户使用：

1. 在 ChatGPT、Claude 或 Gemini 原对话中点击绿色 P。
2. 复制简短续聊码。
3. 在任一支持平台的新 Chat 空白输入框粘贴。
4. Power 取回有原文依据的任务交接内容并自动填入；**由你检查后手动发送**。

同一码可以接续多个目标对话，各目标保留自己的后续任务进度。生成下一份同任务交接码后，旧码失效。

恢复内容是最近有界记录中选出的**任务证据摘录**，不是完整历史或未经核对的 AI 总结。缺失的旧决定、附件、代码和测试记录不能自行猜测。

目前已有模拟浏览器和隔离数据库测试，既有用户报告暂时使用正常；但**尚未通过新用户首次安装和 OAuth 登录的普遍性验收**，也没有正式上架浏览器商店。

## 安全与反馈

不要公开续聊码、密码、API 密钥、Cookie、登录令牌或私人任务内容。

[隐私说明](https://taskonward.5188688.xyz/privacy) · [问题反馈](https://taskonward.5188688.xyz/support)

核心服务仓库保持私有。
