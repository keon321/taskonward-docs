# TaskOnward

**New chat. Same thread.**

TaskOnward helps move the recent working context of a long ChatGPT task into a fresh chat, so you do not have to rebuild the handoff manually.

Start free: https://taskonward.5188688.xyz/

## How it works

1. Install and connect TaskOnward Power.
2. In the old chat, click Power once.
3. Open a new chat and paste the copied continuation text.
4. TaskOnward restores the one-time handoff context.
5. Review the recovery summary.
6. If it is correct, reply `确认`; then give a separate instruction to continue the work.

Replying `确认` only acknowledges the recovery. It does not authorize the assistant to continue the original task automatically.

## Current version

Current: **Power 0.8.8**

The public repository keeps:

- Power 0.8.8 — current; user-reported Chrome Power click accepted;
- Power 0.8.7 — latest rollback;
- Power 0.8.6 — legacy compatibility download.

Older public installation packages may remain available for compatibility. Cross-chat complete resume E2E for 0.8.8 has not been independently verified.

[Power installation guide](docs/power-browser-assistant.md)

## What TaskOnward stores

The current Continuity Lite path keeps exact task identity plus a bounded, temporary handoff snapshot from the explicit Power click. It is not a full transcript archive and does not maintain a second long-term copy of the conversation.

Ordinary ChatGPT use does not continuously upload conversation content to TaskOnward.

## Public beta

TaskOnward is currently free during the public beta. No paid price has been announced.

## FAQ

### How is TaskOnward different from "just ask the model to summarize"?

A normal summary compresses "what we talked about" — it can't tell "decided" from "mentioned", "done" from "doing", or "rejected" from "never raised". TaskOnward saves a structured project state — goal, focus, confirmed decisions, completed work, rejected approaches, next step — and asks you to review and confirm it in the new chat before continuing.

### Does the extension keep recording my chats in the background?

No. During normal chatting, Power stays dormant: no collection, no polling, no auto-saving. It only reads the current conversation the moment you click Power, generating a one-time handoff code.

### Is my full chat history uploaded?

No. Only the bounded state needed for the one-time handoff is uploaded — never the full Conversation JSON, never your ChatGPT cookies, session or access tokens. Handoff codes are single-use and expire after use.

### Why do I have to confirm before resuming?

Because a wrong project state costs more than no state. The restored state is shown to you for review first; you continue only after confirming it's right. Your confirmation just means "this state looks correct" — it doesn't authorize the model to keep executing the original task. What happens next always waits for your explicit instruction.


## Security

Do not publish continuation tokens, passwords, API keys, authentication cookies, private task content, or other secrets.

Privacy: https://taskonward.5188688.xyz/privacy

The core service repository remains private.

[中文说明](README.zh-CN.md)
