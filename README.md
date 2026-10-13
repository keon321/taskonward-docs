# TaskOnward

**New chat. Keep the right task.**

TaskOnward helps carry the current working context into a fresh AI conversation, without asking you to reconstruct the latest decisions and next steps from scratch.

[Get started](https://taskonward.5188688.xyz/start) · [中文说明](README.zh-CN.md)

## Available releases

| Version | Audience | Status |
|---|---|---|
| **Power 0.8.8** | ChatGPT | Current public download |
| **Cross-platform Power 0.4.6** | ChatGPT, Claude, Gemini | Limited observation with existing authorized users |
| Power 0.8.7 | ChatGPT | Stable rollback |

Power 0.4.6 is **not yet a general public installation**. A newly unpacked Chrome extension can receive a different extension ID, while the WorkOS login callback is registered for the existing observation installation. Until fixed-ID distribution and fresh-install OAuth are verified, the website download remains **0.8.8**.

[Power installation guide](docs/power-browser-assistant.md)

## Public Power 0.8.8

1. Install Power and sign in.
2. Open the current ChatGPT conversation and click Power.
3. Paste the copied handoff into a new Chat.
4. Review the restored working context before giving another instruction.

The handoff is bounded and temporary. It is not a full transcript archive or a second permanent project-memory database. Ordinary chatting does not continuously upload messages.

## Cross-platform Power 0.4.6 (limited observation)

For users who already have an authorized observation installation:

1. Click the green P in an existing ChatGPT, Claude, or Gemini chat.
2. Copy the short TaskOnward code.
3. Paste it into an empty input box in a new chat on any supported platform.
4. Power retrieves an **evidence-based task handoff**, fills the input, and waits for you to review and send it manually.

The same code can be used in multiple destination chats. Each destination retains its own subsequent working branch under the same task identity. Generating a new handoff for that task invalidates the earlier code.

The handoff is an extract from bounded, verified message evidence—not a guaranteed complete or lossless historical summary. It must not invent missing decisions, files, or project milestones.

The current observation code has passed simulated Chromium and isolated database tests; early users report it working, but general fresh-install and OAuth reliability are **not yet verified**.

## Security and support

Do not share handoff codes, passwords, API keys, authentication cookies, private task content, or OAuth tokens.

[Privacy](https://taskonward.5188688.xyz/privacy) · [Support](https://taskonward.5188688.xyz/support)

The core service repository remains private. No browser-store publication is claimed.
