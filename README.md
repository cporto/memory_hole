# Memory Hole

Every time you start a new conversation with an AI, it has no idea who you are. You end up re-explaining yourself — your tools, your preferences, decisions you've already made, how you like to work.

Memory Hole fixes that.

It's a set of plain text files you own and maintain. At the start of any AI conversation, you load those files in. The AI immediately knows who you are, how you work, and what you're working on. No re-explaining.

It works with any AI — Claude, ChatGPT, Gemini, or a local model. You're not locked into anything.

---

## How it works

- **You own the files.** Plain markdown. No app, no subscription, no vendor lock-in.
- **You load them in.** Upload or paste at the start of a session. The AI picks up where you left off.
- **You save updates back.** At the end of a session, say `update memory hole`. The AI outputs ready-to-paste updates. You copy and save them.
- **Works offline.** Files live on your device. Use with a local LLM and no internet required.

---

## What's in this repo

| File | What it is |
|------|-----------|
| `ONBOARDING.md` | Run this once to generate your personal files |
| `START_MEMORY_HOLE.md` | Your session starter — load this at the beginning of every conversation |
| `GUIDE.md` | Full setup and usage guide |
| `SYSTEM.md` | How the update trigger and decision capture logic works |

---

## Getting started

1. Read **[GUIDE.md](GUIDE.md)** first — it covers storage setup, mobile access, and your daily workflow
2. Download the files: **[Download ZIP](https://github.com/cporto/memory_hole/archive/refs/heads/main.zip)** — unzip and you're ready. If you know how to use git, clone the repo instead.
3. Open an AI chat tool — [Claude](https://claude.ai), [ChatGPT](https://chatgpt.com), [Gemini](https://gemini.google.com), or any other — and upload `ONBOARDING.md` from the folder you just downloaded or cloned into a new conversation
4. The AI will start interviewing you — answer each question as it comes. At the end, it generates two files: `WHO_I_AM.md` (your profile) and `START_MEMORY_HOLE.md` (your session starter)
5. Save those two files to your repo or folder
6. Load `START_MEMORY_HOLE.md` at the start of any AI conversation — you're live

---

## Requirements

Nothing. Plain text files, any AI, any device.

---

## What never goes in Memory Hole

Passwords, credentials, financial details, medical information. Context and reasoning only.

---

## License

MIT
