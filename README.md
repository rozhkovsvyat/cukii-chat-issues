# Cukii Chat

![Cukii Chat](https://raw.githubusercontent.com/rozhkovsvyat/cukii-chat-issues/main/media/icon.png)

One VS Code chat for the coding CLIs you already pay for — Claude Code, Codex,
Kimi Code, Qwen Code, Grok and Cursor agent. Cukii Chat spawns the real vendor
CLI under your own subscription and turns its stream into a single chat feed:
tool calls, diffs, follow-ups mid-turn, usage limits, reactions, sticky prompt
capsules.

**[Install from the VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=cukii.cukii-vscode)**

## This repository

This is the public issue tracker and landing page for Cukii Chat. The source
code is developed privately; releases ship through the Marketplace and the
changelog on the listing page.

- **Bug or regression?** [Open an issue](../../issues/new/choose). The fastest
  way is **Report a bug** inside the chat — it attaches the diagnostics the
  team needs and drops you here with everything pre-filled.
- **IDEs without the Microsoft Marketplace** (Cursor, Windsurf, VSCodium):
  grab the `.vsix` for your platform from the listing's version history or ask
  in an issue — an Open VSX publication is on the roadmap.

## Requirements

- VS Code 1.70+, a **trusted workspace** (the extension is off in Restricted
  Mode, because agents execute real commands).
- At least one vendor CLI signed in with your own subscription or key. Cukii
  Chat never asks for your vendor tokens itself — the CLIs own their
  credentials.

## Privacy

Bug reports you send from the chat include a screenshot of the visible chat,
the diagnostics log and the versions involved — nothing else leaves the
machine, and nothing is sent unless you press the button. There is no
telemetry in the extension.
