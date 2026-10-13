# Power 浏览器助手｜安装与使用

当前公开下载是 **Power 0.8.8（ChatGPT）**。跨平台 0.4.6 仍在小范围观察，不提供面向新用户的通用安装。

## 先了解两种版本

| | 公开稳定版 0.8.8 | 跨平台观察版 0.4.6 |
|---|---|---|
| 平台 | ChatGPT | ChatGPT、Claude、Gemini |
| 原对话生成交接 | 点击 Power | 点击绿色 P |
| 新对话恢复 | **需要 ChatGPT 已连接 TaskOnward MCP** | 浏览器扩展自动取回 |
| 同一码使用 | 旧版单目标规则 | 多个目标对话，生成新码后旧码失效 |
| 公开下载 | **提供** | **暂不提供** |

**MCP 的准确作用：** 公开 0.8.8 中，Power 在旧对话负责准备交接码；目标 ChatGPT 中的 TaskOnward MCP 通过 `resume_handoff` 读取交接。**不能只连接 MCP、在旧对话发送“保存这个任务并准备续聊”来生成交接码。**

## 公开版 0.8.8 安装

[下载 Power 0.8.8 ZIP](../downloads/taskonward-power-0.8.8.zip)

SHA-256：`600c77c86a7f4ff054fdd05dc20cda403c5280cdbbf14cabba52e0d6b8e2a7d5`

1. 下载 ZIP 并解压到固定文件夹。
2. 打开 Chrome 地址栏中的 `chrome://extensions/`。
3. 打开页面右上角**开发者模式**，点击**加载已解压的扩展程序**。
4. 选择包含 `manifest.json` 的 Power 0.8.8 文件夹。
5. 点击浏览器工具栏中的 Power，用 TaskOnward 账号完成登录，刷新 ChatGPT 网页。

Chrome 扩展页的“开发者模式”和 ChatGPT 内的开发者模式是不同的设置。

## 在 ChatGPT 连接 TaskOnward MCP（0.8.8 恢复必需）

1. 进入 ChatGPT 设置，找到 Apps / Connectors（名称可能因账号和工作区而不同）。
2. 如果账号提供自定义连接功能，在对应设置中添加 TaskOnward，服务地址填写：

   `https://taskonward.5188688.xyz/mcp`

3. 按提示完成 TaskOnward 的 OAuth 登录授权。尽量使用与 Power 相同的 TaskOnward 账号。

**如果 ChatGPT 未提供自定义连接入口、无法完成授权或未成功连接 TaskOnward，就不能把 0.8.8 的短码当成已经恢复。** 仅安装 Power 不能代替目标 ChatGPT 的 MCP 恢复功能。

## 实际续聊

1. 在原 ChatGPT 对话中点击 Power，等待提示复制成功。
2. 自己打开新的 ChatGPT 对话，粘贴交接内容并发送。
3. 确认新对话**真正调用 TaskOnward 并取回当前交接**，而不是只重复短码或猜测历史。
4. 核对最近完成事项、未解决问题和下一步。如果恢复不正确，指出缺失或错误；确认正确后，再明确告诉 AI 要做什么。

Power 不自动打开新聊天，也不自动发送消息；普通聊天时不持续采集。交接只是有界的最近任务现场，不保证包含完整聊天、附件、全部已确认决定或长期状态。

## 跨平台观察版 0.4.6

已安装且获授权的观察用户：在 ChatGPT、Claude 或 Gemini 原对话点绿色 P，复制短码；在目标 Chat 的空白输入框粘贴，扩展自动取回任务原文证据摘录并填入，由用户手动发送。**目标 AI 不需要单独安装 TaskOnward MCP。**

目前 **不开放新用户直接下载观察版 ZIP**：新安装目录可能导致不同 Chrome 扩展 ID，而登录回调只登记了现有观察安装的 ID。要先完成固定 ID、OAuth 回调及全新安装验收。

## 下载及安全

- 0.8.8：当前公开下载。
- 0.8.7：可回退的旧版。
- 0.8.6：现有兼容下载；不是新用户推荐版本。

请勿公开续聊码、登录令牌、密码、API Key、Cookie 或私人任务内容。出现问题时请提供平台、版本、时间和去敏截图，不要把交接全文贴到公开 Issue。
