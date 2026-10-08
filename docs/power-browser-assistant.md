# Power 浏览器助手｜手动安装

Power 是 TaskOnward 的可选浏览器助手。

它只负责把当前 Chat 的最近任务现场做成一次性交接内容并复制到剪贴板。你再打开新 Chat，粘贴发送即可。TaskOnward 不再维护第二套长期内容记忆。Power 0.8.8 继续使用自有 API 域名与单阶段续聊：新 Chat 只需调用一次 `resume_handoff`。点击 Power 时只冻结一次页面 witness，并同时读取 ChatGPT 当前活动分支；API 只保留用户真正可见的 user/assistant turn，过滤工具与隐藏节点。API 已比页面 witness 更新时直接采用，API 落后时只重试 API（遇到 429 限流立即转已冻结的可信 DOM），不会重读页面。DOM fallback 优先识别能证明角色的语义节点，不再按 turn 顺序猜 user/assistant；完全读不到可信现场时会停止，并显示一个不含聊天正文的短诊断编号。

## 下载

[下载 TaskOnward Power 0.8.8 ZIP](../downloads/taskonward-power-0.8.8.zip)

SHA-256：

`600c77c86a7f4ff054fdd05dc20cda403c5280cdbbf14cabba52e0d6b8e2a7d5`

最近回滚包 Power 0.8.7；新安装始终使用 0.8.8。0.8.6 旧版下载仍保留兼容。

## Chrome 安装

1. 下载 ZIP，并解压；
2. 打开 `chrome://extensions/`；
3. 打开开发者模式；
4. 加载已解压的扩展程序；
5. 选择解压后的文件夹；
6. 刷新 ChatGPT。升级已有 Power 时也请刷新已打开的 ChatGPT 页面一次，避免旧扩展页面脚本继续停留在旧上下文。

## 使用

准备换 Chat 时：

1. 点击 Power；
2. 复制续聊内容；
3. 打开新 Chat；
4. 粘贴发送；
5. 检查恢复摘要；正确则回复「确认」，不正确就直接指出需要修改的地方；
6. 回复「确认」只表示你认可这次交接；不需要再调用 TaskOnward。你明确说「继续」或给出下一条任务指令后，才继续原任务。

Power 不会自动打开新 Chat，也不会自动发送消息。

Power 0.8.8 已完成自动化门禁与线上包校验，并由用户报告原 Chrome 扩展点击成功。此结果仅证实 Power 点击可用，**不代表“新 Chat 粘贴并完整恢复”已经过端到端验收**。手动安装版升级后需要在 Chrome 扩展页重新加载扩展并刷新 ChatGPT。

## 安全提醒

不要把密码、API Key、Cookie、OAuth 令牌或续聊令牌发给别人。
