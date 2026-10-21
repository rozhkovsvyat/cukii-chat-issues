# Cukii Chat

![Cukii Chat](https://raw.githubusercontent.com/rozhkovsvyat/cukii-chat-issues/main/media/icon.png)

One VS Code chat for the coding CLIs you already pay for — Claude Code, Codex,
Kimi Code, Qwen Code, Grok and Cursor agent. Cukii Chat runs the real vendor
CLI under your own subscription and shows it as one chat.

**[Install from the VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=cukii.cukii-vscode)**

## This repository

This is the public issue tracker and landing page. The source is developed
privately. Releases ship through the Marketplace and the changelog on the
listing page.

- **Bug or regression?** [Open an issue](../../issues/new/choose). No team
  invitation or repository write access is needed.
- **From the extension:** **Commands and model → Report an issue…**. Sign in
  with GitHub through VS Code, review the report, then press **Send**.
- **IDEs without the Microsoft Marketplace** (Cursor, Windsurf, VSCodium):
  take the `.vsix` from the listing's version history or ask in an issue. An
  Open VSX publication is on the roadmap.

## Requirements

- VS Code 1.70 or newer, and a trusted workspace. The extension stays off in
  Restricted Mode because the agents run real commands.
- One vendor account you already pay for. **Manage accounts → Install**
  downloads that CLI. On macOS and Linux you need `curl` and `tar`; Install
  downloads Node.js for you. On Windows, Install uses `npm` if it is on
  `PATH`, or installs the current Node.js LTS with winget.
- In a Remote-SSH window, install and sign in there. The CLI runs in the
  remote user's home. The sign-in page opens on your local computer. If it
  does not, copy the `https` link from the login terminal, or for Codex from
  the Output channel **Cukii Chat · codex login**.

## Existing reports

The first migration brought 68 open reports and 81 historical comments from
the former private tracker. Their 113 reviewed attachments use immutable links
and were checked by SHA-256. Seven screenshots with personal or private
project information stay withheld. Closed historical cards remain in the
private archive.

## Privacy

GitHub issues and the files linked from them are public.

The in-chat form shows your text, a chat snapshot, any screenshots and masked
diagnostic logs before publication. You can remove the snapshot. Masking does
not read screenshots; check them yourself.

Signing in does not publish a report. Review the text and files, then press
**Send**. Pressing **Send** publishes them publicly. VS Code requests the
GitHub scopes `public_repo` and
`read:user`. `public_repo`
is broader than this one repository. The reporter sends the files and an
OAuth token over HTTPS to `cukii.shop`. The intake uses the token
only to verify you and create the issue here. It does not store or log the
token. You can instead open an issue directly on GitHub.

No telemetry is on by default. Reports queued privately on your machine stay
in a separate local archive. Historical cards from the private tracker are
published only after a separate privacy review.
