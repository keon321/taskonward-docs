# Power 浏览器助手｜手动安装

Power 是 TaskOnward 的可选浏览器助手。

它只负责把当前 Chat 的最近任务现场做成一次性交接内容并复制到剪贴板。你再打开新 Chat，粘贴发送即可。TaskOnward 不再维护第二套长期内容记忆。Power 0.8.5 继续使用自有 API 域名与单阶段续聊：新 Chat 只需调用一次 `resume_handoff`。用户回复「确认」只是聊天层面的确认，不再触发第二个 TaskOnward 工具调用。0.8.5 把“读到当前对话”改成前置硬门禁：先读 ChatGPT 当前分支；主路径失败时最多做 3 次短 DOM 重试；只有同时读到用户请求和 ChatGPT 回答才允许生成续聊。读到后立即冻结同一份现场，服务异常时不再二次读取。

## 下载

[下载 TaskOnward Power 0.8.5 ZIP](../downloads/taskonward-power-0.8.5.zip)

SHA-256：

`649616ec01bb2552180b0b4bca609ad0679f6a8263707df46c7ed3f83fb24e6b`

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

## 安全提醒

不要把密码、API Key、Cookie、OAuth 令牌或续聊令牌发给别人。
