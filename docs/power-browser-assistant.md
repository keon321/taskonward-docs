# Power 浏览器助手｜手动安装

Power 是 TaskOnward 的可选浏览器助手。

它只负责把当前 Chat 的最近任务现场做成一次性交接内容并复制到剪贴板。你再打开新 Chat，粘贴发送即可。TaskOnward 不再维护第二套长期内容记忆。Power 0.8.4 继续使用自有 API 域名与单阶段续聊：新 Chat 只需调用一次 `resume_handoff`。用户回复「确认」只是聊天层面的确认，不再触发第二个 TaskOnward 工具调用。0.8.4 同时修复服务不可用时的本地应急回退：本次 Power 点击已经取得的最新现场优先，额外 DOM 应急补读只补缺口，不能把最新现场回退为空或较旧内容。

## 下载

[下载 TaskOnward Power 0.8.4 ZIP](../downloads/taskonward-power-0.8.4.zip)

SHA-256：

`ae2f233145029be26de7911abb67f8e20169d33a8eadc1d0d3789526fed76aaf`

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
