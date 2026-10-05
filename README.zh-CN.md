# TaskOnward

**换一个新对话，继续刚才的工作。**

TaskOnward 用来把长 ChatGPT 对话里**最近的工作现场**交接到新 Chat，避免每次重新解释。

## 怎么用

1. 安装并连接 TaskOnward Power；
2. 在旧 Chat 点一次 Power；
3. 打开新 Chat，粘贴自动复制的续聊内容；
4. TaskOnward 恢复这次点击冻结的交接现场；
5. 检查恢复摘要；
6. 正确就回复「确认」，然后再单独给出「继续」或下一条具体指令。

「确认」只表示恢复正确，不代表授权模型自动继续原任务。

## 当前版本

当前版本：**Power 0.8.6**

公开仓只保留：

- 0.8.6：当前版本；
- 0.8.5：最近回滚。

更旧公开安装包已清理，不再作为新用户入口。

[Power 安装说明](docs/power-browser-assistant.md)

## 保存什么

当前 Continuity Lite 只保存精确任务身份，以及用户点击 Power 时生成的**有界、临时一次性交接现场**。

它不是完整聊天归档，也不再维护第二套长期任务内容记忆。普通 ChatGPT 使用期间，不会持续把对话内容上传到 TaskOnward。

## 当前免费测试

公开测试阶段目前免费，尚未公布正式付费价格。

## 免费开始

https://taskonward.5188688.xyz/start

## 安全

不要公开续聊码、密码、接口密钥、Cookie、OAuth 令牌、私人任务内容或其他秘密。

隐私说明：

https://taskonward.5188688.xyz/privacy

核心服务源码保持私有。
