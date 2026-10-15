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

- **Bug or regression?** [Open an issue](../../issues/new/choose). No YouGile
  account, team invitation or repository write access is needed.
- **Integrated reporting preview:** candidate 2.0.183 adds **Commands and model
  → Report an issue…** with GitHub sign-in, reviewed screenshots and diagnostic
  logs. This candidate is still in acceptance; it is not yet the Marketplace
  release. Until it ships, use the GitHub issue form directly.
- **IDEs without the Microsoft Marketplace** (Cursor, Windsurf, VSCodium):
  grab the `.vsix` for your platform from the listing's version history or ask
  in an issue — an Open VSX publication is on the roadmap.

## Requirements

- VS Code 1.70+, a **trusted workspace** (the extension is off in Restricted
  Mode, because agents execute real commands).
- At least one vendor CLI signed in with your own subscription or key. Cukii
  Chat keeps credentials on your machine: CLI sign-ins stay with the CLIs;
  API keys use VS Code secret storage.

## Existing reports

The first migration wave brought 68 open reports and 81 historical comments
from the former private tracker. Their 113 reviewed attachments use immutable
links and were verified by SHA-256. Seven screenshots containing personal or
private project information are explicitly withheld. Closed historical cards
remain in the private archive for a later migration phase.

## Privacy

GitHub issues and their attachments are public. The upcoming in-chat reporter shows the
chat snapshot, optional screenshots and masked diagnostic logs before you
publish. Check images and text for private information; automatic masking
cannot recognize everything in a screenshot. You can remove the chat snapshot.

GitHub sign-in uses VS Code's built-in provider. Publishing through the in-chat
reporter sends the selected files and a temporary GitHub OAuth token over HTTPS
to `cukii.shop`. The intake uses the token only to verify the sender and create
the report in this repository; it does not store or log the token. VS Code
requests GitHub's `public_repo` scope, which is broader than this single
repository. You can instead submit an issue directly on GitHub.

Signing in alone does not publish a report. Publication requires the explicit
public-consent checkbox and **Publish on GitHub**. There is no telemetry enabled
by default. Historical reports from the former private tracker are migrated
only after a separate privacy review; original private evidence is not
automatically published.
