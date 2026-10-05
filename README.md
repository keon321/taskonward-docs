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

Current: **Power 0.8.6**

The public repository keeps:

- Power 0.8.6 — current;
- Power 0.8.5 — latest rollback.

Older public installation packages are intentionally removed.

[Power installation guide](docs/power-browser-assistant.md)

## What TaskOnward stores

The current Continuity Lite path keeps exact task identity plus a bounded, temporary handoff snapshot from the explicit Power click. It is not a full transcript archive and does not maintain a second long-term copy of the conversation.

Ordinary ChatGPT use does not continuously upload conversation content to TaskOnward.

## Public beta

TaskOnward is currently free during the public beta. No paid price has been announced.

## Security

Do not publish continuation tokens, passwords, API keys, authentication cookies, private task content, or other secrets.

Privacy: https://taskonward.5188688.xyz/privacy

The core service repository remains private.

[中文说明](README.zh-CN.md)
