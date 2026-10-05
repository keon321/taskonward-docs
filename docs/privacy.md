# Privacy summary

TaskOnward Continuity Lite is designed as a bounded task-handoff bridge, not a full transcript archive.

## Current handoff data

When the user explicitly clicks Power, the service may temporarily store:

- exact task identity and conversation binding metadata;
- a bounded recent-message snapshot needed for the one-time handoff;
- minimal timestamps and status needed to deliver and expire that handoff.

Ordinary ChatGPT use does not continuously upload conversation content to TaskOnward.

## Data protection

- User data is tenant-isolated.
- Temporary handoff payloads are encrypted.
- Handoff content is bounded rather than a full conversation archive.
- Consumed or expired temporary payloads are scrubbed by the current lifecycle.

## Secrets

Do not include passwords, API keys, seed phrases, authentication cookies, access tokens, or other secrets in a TaskOnward handoff or public bug report.

Full current notice:

https://taskonward.5188688.xyz/privacy
