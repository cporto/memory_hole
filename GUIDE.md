# Memory Hole — How to Use It

---

## What is Memory Hole?

Every time you start a new conversation with an AI, it has no idea who you are. You end up re-explaining yourself over and over — your tools, your preferences, decisions you've already made, how you like to work.

Memory Hole fixes that. It's a set of plain text files you own and maintain. At the start of any AI conversation, you upload those files in. The AI immediately knows who you are, how you work, and what you're working on. No re-explaining.

It works with any AI — Claude, ChatGPT, Gemini, or a local model. You're not locked into anything.

---

## Contents

- [Before you start — pick your storage](#before-you-start--pick-your-storage)
- [GitHub Setup](#github-setup)
  - [1. Create a GitHub account](#1-create-a-github-account)
  - [2. Create a new repository](#2-create-a-new-repository)
  - [3. Add your first file](#3-add-your-first-file)
  - [4. Editing a file later](#4-editing-a-file-later)
  - [5. On Mobile](#5-on-mobile)
  - [6. On Mac or Windows](#6-on-mac-or-windows)
- [Step 1 — Run the onboarding interview](#step-1--run-the-onboarding-interview)
- [Step 2 — Your daily workflow](#step-2--your-daily-workflow)
  - [Starting a new conversation](#starting-a-new-conversation-no-specific-project)
  - [Working on a project](#working-on-a-project)
  - [Capturing research](#capturing-research)
  - [Logging decisions](#logging-decisions)
  - [Pulling in extra context](#pulling-in-extra-context)
- [Keeping your memory clean](#keeping-your-memory-clean)
- [Keeping your profile up to date](#keeping-your-profile-up-to-date)
- [What "update memory hole" does](#what-update-memory-hole-does)
- [What never goes in Memory Hole](#what-never-goes-in-memory-hole)
- [File reference](#file-reference)
- [Common mistakes](#common-mistakes)

---

## Before you start — pick your storage

Memory Hole needs somewhere to live. There are two options.

### Option A — GitHub (recommended)

GitHub (**[github.com](https://github.com)**) is a free service that stores your files online, keeps a full history of every change, and lets you access them from any device. This is the recommended option because if you ever overwrite something by mistake, you can go back. You also always have a backup that isn't tied to one device.

→ If you're going with GitHub, follow the setup steps in the next section before anything else.

### Option B — Local folder only

If GitHub feels like too much right now, you can skip it. Create a folder on your computer or in [iCloud](https://icloud.com) / [Google Drive](https://drive.google.com) / [Dropbox](https://dropbox.com) — wherever you already store files — and use that instead.

What you give up: there's no version history. If you overwrite a file by mistake, it's gone. This is fine for getting started and testing — you can always migrate to GitHub later.

→ If you're going with a local folder, skip the GitHub setup section and go straight to [Step 1 — Onboarding](#step-1--run-the-onboarding-interview).

---

## GitHub Setup

Before anything else, download the Memory Hole starter files: **[Download ZIP](../../archive/refs/heads/main.zip)**

The folder contains all the files referenced in this guide — including `ONBOARDING.md`, which you'll need in Step 1.

This section then walks you through creating your GitHub account and setting up your own Memory Hole repository. You only do this once.

---

### 1. Create a GitHub account

Go to **[github.com](https://github.com)** and click **Sign up**.

> *[screenshot: GitHub homepage with Sign up button highlighted]*

Follow the prompts to create your account. A free account is all you need — don't pay for anything.

---

### 2. Create a new repository

A repository (or "repo") is just a folder on GitHub where your files will live.

Once you're logged in, click the **+** icon in the top right corner of the page, then click **New repository**.

> *[screenshot: GitHub top navigation with + icon and "New repository" option highlighted]*

Fill in the details:

- **Repository name:** `memory-hole`
- **Description:** optional — you can leave it blank
- **Visibility:** set to **Private** — this means only you can see it

> *[screenshot: New repository form with name field, and Private option selected]*

Click **Create repository**.

---

### 3. Add your first file

After the interview (Step 1 below), you'll have two files to save here. Here's how to add a file to your repo:

On your repository page, click **Add file**, then click **Create new file**.

> *[screenshot: Repository page with "Add file" button highlighted]*

Name the file exactly as shown — `WHO_I_AM.md` — then paste your content into the editor below. The filename must match exactly for the system to work.

> *[screenshot: New file editor with filename field and content area highlighted]*

When you're done, scroll down and click **Commit changes**. You can leave the commit message as-is.

> *[screenshot: Commit changes button at bottom of file editor]*

"Committing" just means saving. Every time you commit, GitHub takes a snapshot of the file at that moment — so you can always go back to an earlier version if something goes wrong.

That's it. The file is saved.

---

### 4. Editing a file later

When you need to update a file after a session, click the file name to open it, then click the **pencil icon** in the top right of the file view to edit it.

> *[screenshot: File view with pencil/edit icon highlighted]*

Paste in your updated content, then click **Commit changes** to save.

---

### 5. On Mobile

---

#### iPhone or iPad

You have two options depending on where your Memory Hole files live.

---

**Option A — GitHub (Working Copy)**

If you're using GitHub to store your files, install **[Working Copy](https://workingcopyapp.com)** — available on the App Store at **workingcopyapp.com** or search "Working Copy." It connects to your GitHub account and mounts your repository directly into the iOS Files app — so you can access and upload your memory files the same way you'd open any document on your phone.

> **Note:** GitHub also has an iOS app, but it's not what you need here — it's built for managing code projects, not editing files. Use Working Copy instead.

To connect Working Copy to GitHub:
1. Open Working Copy and tap the **+** icon
2. Select **Clone repository**
3. Tap **GitHub** and sign in with your GitHub account when prompted
4. Select your `memory-hole` repository from the list
5. Once cloned, your files will appear inside the iOS Files app under Working Copy

> **Sync before you start.** Before uploading any files into a session, open Working Copy and pull the latest version of your repository. If you've edited files on another device since last time, this ensures you're not working from stale memory.

> *[screenshot: Working Copy app in App Store]*

> *[screenshot: Working Copy clone repository screen with GitHub option highlighted]*

> *[screenshot: Memory Hole repo visible inside iOS Files app]*

---

**Option B — Local storage (iCloud, Google Drive, Dropbox, OneDrive)**

If you're storing your Memory Hole files in a cloud folder instead of GitHub, you can access them directly from the iOS Files app — no extra tools needed for iCloud. For Google Drive, Dropbox, or OneDrive, install their respective iOS apps first and they'll appear as locations inside Files automatically.

To access your files:
1. Open the **Files** app on your iPhone or iPad
2. Navigate to the folder where your Memory Hole files are stored — this will be under iCloud Drive, Google Drive, Dropbox, or OneDrive depending on what you use
3. Tap and hold the file, then tap **Share** to upload it directly into your AI app of choice

> **If your AI app doesn't support file uploads**, tap the file to open it, select all, copy, and paste into the conversation instead.

> **Sync before you start.** If you've edited files on another device since last time, make sure your cloud storage has finished syncing before uploading any files into a session. Loading stale memory into an AI conversation is the most common way to lose context.

---

#### Android

Android support depends on where your Memory Hole files live.

---

**If you're using GitHub:** there is currently no Android app equivalent to Working Copy that cleanly mounts a GitHub repository into the file system. The most reliable option for Android GitHub users is the browser — go to **[github.com](https://github.com)** in Chrome or your preferred browser, open your `memory-hole` repository, and copy file contents from there to paste into your AI app.

> We're aware this is a gap. Android's openness means better tools are likely to emerge — we'll update this section when a clean solution exists.

---

**If you're using local storage (Google Drive, Dropbox, OneDrive):** install the relevant app from the Play Store and your files will be accessible through the Android file picker. Most AI apps on Android support file uploads directly from Google Drive or local storage.

To access your files:
1. Open your AI app and look for the file upload or attachment option
2. Navigate to your Memory Hole folder in Google Drive, Dropbox, or OneDrive
3. Select the file to upload it directly into the conversation

> **If your AI app doesn't support file uploads**, open the file in Google Drive or your storage app of choice, select all, copy, and paste into the conversation instead.

> **Sync before you start.** Make sure your cloud storage app has finished syncing before uploading any files into a session. Loading stale memory into an AI conversation is the most common way to lose context.

---

### 6. On Mac or Windows

You have two options depending on how you want to work.

---

**Option A — Browser only (no install needed)**

The simplest option. GitHub has a built-in editor — you can create and edit files directly on github.com in any browser, on any computer. No software to install.

To edit a file:
1. Go to **[github.com](https://github.com)** and open your `memory-hole` repository
2. Click the file you want to edit
3. Click the **pencil icon** in the top right of the file view
4. Make your changes, then click **Commit changes** to save

This works anywhere — Mac, Windows, a library computer, doesn't matter. The only limitation is that you need an internet connection.

---

**Option B — Local files on your computer (one tool)**

If you want your memory files available offline, or you prefer editing in a proper text editor, install **[GitHub Desktop](https://desktop.github.com)** — a free app made by GitHub, available for both Mac and Windows.

GitHub Desktop syncs your GitHub repository to a folder on your computer. You edit the files locally in any text editor, then use GitHub Desktop to push the changes back to GitHub.

To set it up:
1. Download and install **GitHub Desktop** from **[desktop.github.com](https://desktop.github.com)**
2. Open the app and sign in with your GitHub account
3. Click **File → Clone repository**
4. Select your `memory-hole` repository from the list
5. Choose where to save it on your computer and click **Clone**

> *[screenshot: GitHub Desktop clone repository screen with memory-hole repo selected]*

Your files are now on your computer. You can open and edit them in any text editor — TextEdit on Mac, Notepad on Windows, or whatever you prefer.

After editing, push your changes back to GitHub:
1. Open GitHub Desktop — it will show the files you changed
2. Add a short note in the **Summary** field (e.g. "session update")
3. Click **Commit to main**, then click **Push origin**

> *[screenshot: GitHub Desktop showing changed files, commit summary field, and Push origin button]*

That's it — your changes are saved to GitHub and backed up.

> **Sync before you start.** If you've edited files on another device since last time, click **Fetch origin** in GitHub Desktop before opening any files. This pulls down the latest version so you're not working from stale memory.

---

## Step 1 — Run the onboarding interview

This is a one-time step. It generates the two core files you need to use the system.

1. Open any AI tool — [Claude](https://claude.ai), [ChatGPT](https://chatgpt.com), [Gemini](https://gemini.google.com), your choice
2. Upload `ONBOARDING.md` directly into a new AI conversation
3. The AI will start interviewing you — answer each question as it comes. At the end, it generates two files: `WHO_I_AM.md` (your profile) and `START_MEMORY_HOLE.md` (your session starter)
4. Copy each file's contents and save them to your GitHub repo or local folder using the steps above. The filenames must be named exactly as shown — `WHO_I_AM.md` and `START_MEMORY_HOLE.md` — for the system to work.

> **If your AI doesn't support file uploads**, open `ONBOARDING.md` in any text editor, copy the entire contents, and paste it into the conversation instead.

You only run onboarding once. After this, `ONBOARDING.md` is no longer needed.

---

## Step 2 — Your daily workflow

### Starting a new conversation (no specific project)

Your files are plain text — you can open them in any text editor (Notes app, TextEdit on Mac, Notepad on Windows). On mobile, refer to the setup section above for how to access your files on iOS or Android.

> **Sync before you start.** If you've edited files on another device since last time, make sure you have the latest version before copying anything. Stale memory loaded into an AI conversation means the AI is working from outdated context.

1. Upload `START_MEMORY_HOLE.md` directly into a new AI conversation
2. Work normally — the AI already knows who you are

> **If your AI doesn't support file uploads** (some local LLMs and simpler interfaces), open `START_MEMORY_HOLE.md` in any text editor, copy the entire contents, and paste it into the conversation instead.

At the end of your session, say: **"update memory hole"**

The AI generates formatted updates for any files that changed. Copy those updates and save them back to your repo or folder.

---

### Working on a project

Here's what a typical project setup looks like:

```
projects/
  my-website-redesign/
    project.md        ← always exists
    research.md       ← split out automatically when research gets large
    decisions.md      ← split out automatically when decisions get large
  another-project/
    project.md
```

Project files live in a `projects/` folder inside your repo or local folder. You'll need to create this folder yourself the first time. Each project then gets its own subfolder inside it — create that too when you start a new project, for example `projects/my-website-redesign/`.

Inside each project folder lives a single `project.md` file. This is where everything starts — current state, decisions, research notes. As your project grows, the AI will automatically split research and decisions into their own files (`research.md`, `decisions.md`) inside the same project folder when they get large enough to warrant it.

If a new project comes up during a session, the AI will flag it and offer to create a project file. At the end of the session, say "update memory hole" — the AI will include the new project file in the output. Copy that output and save it as `project.md` inside a new subfolder in `projects/` — for example, `projects/my-website-redesign/project.md`.

To work on an existing project:

1. Upload `START_MEMORY_HOLE.md` and `project.md` from your project subfolder into a new AI conversation
2. Work — the AI knows your identity, your project state, open questions, and decisions already made. It won't re-open things you've already settled.

> **If your project has split files** (`research.md` or `decisions.md`), you don't need to load them upfront. Only upload them mid-session if the work specifically requires digging into research or reviewing past decisions. Load what's relevant, when it's relevant.

> **If your AI doesn't support file uploads**, open each file in a text editor, copy the contents, and paste them in separately.

Once you're done working, say **"update memory hole"** to capture everything from the session. The AI will output an updated version of your project file reflecting the current state, any decisions made, and any open questions. Copy that output and save it back to your project subfolder, replacing the previous version.

---

### Capturing research

Any findings that surface during a session — conclusions reached, approaches ruled out, sources worth remembering — are automatically captured in your project file when you say "update memory hole." You don't need to flag them during the session. The AI tracks what came up and includes it in the output.

---

### Logging decisions

Decisions are automatically captured in your project file when you say "update memory hole" — including the reasoning behind them, not just what was decided. You don't need to call them out explicitly. If a decision was made during the session, it will be in the output.

---

### Pulling in extra context

Not everything needs to be loaded at the start of a session. If a topic comes up mid-session that's covered in another project file, upload or paste it into the conversation at that point. Loading too many files upfront shrinks the space the AI has to actually think and work — only bring in what's relevant, when it's relevant.

---

## Keeping your memory clean

Memory files go stale over time — projects finish, research becomes outdated, decisions get reversed. If you never prune your files, the AI starts working with noise instead of signal. A clean memory system is a more useful one.

### What to prune

- **Completed projects** — once a project is fully done and nothing from it is relevant to future work, it doesn't need to stay active
- **Outdated research** — findings that have been superseded or no longer apply
- **Reversed decisions** — if a decision in your project file was undone, remove it rather than letting it sit

### How to prune

**If you're using GitHub:** it's safe to delete files directly. Every change is versioned automatically — if you ever need a deleted file back, it's recoverable from your repo history.

**If you're using a local folder:** don't delete files permanently. Instead, create an `archive/` folder inside your Memory Hole folder and move stale files there. This keeps your active memory clean without losing anything forever.

### When to prune

There's no fixed schedule — just check in occasionally. A good trigger is when a project wraps up, or when you notice you're loading files into sessions that aren't actually useful anymore.

---

## Keeping your profile up to date

Your `WHO_I_AM.md` file is your source of truth. If something about how you work changes — new tools, new preferences, new focus — it should be reflected there.

You can update it two ways. The first is directly — open the file, edit it, and save it back. The second is during a session — mention the change and the AI will include an updated version of `WHO_I_AM.md` in the "update memory hole" output. Either way, you still need to copy the output and save it back to your file manually — nothing saves automatically.

---

## What "update memory hole" does

When you say those three words at the end of a session, the AI generates exact, ready-to-paste updates for every file that changed. You don't have to figure out what to write — just copy what it outputs and save it.

Every update captures:
- What changed and why
- Any decisions made — with the reasoning, not just the outcome
- New open questions
- What was resolved

---

## What never goes in Memory Hole

- Passwords or login credentials
- Financial details
- Medical information

Context and reasoning only. If it's sensitive, keep it out.

---

## File reference

| File | What it is | When you use it |
|------|-----------|----------------|
| `ONBOARDING.md` | The setup interview | Once, at the very beginning |
| `WHO_I_AM.md` | Your profile — source of truth | Update it when things change |
| `START_MEMORY_HOLE.md` | Session starter — upload or paste this every time | Every session |
| `projects/[name]/project.md` | Main file for each project | When working on that project |
| `projects/[name]/research.md` | Research notes — auto-split from project.md when large | On demand, mid-session only |
| `projects/[name]/decisions.md` | Decisions — auto-split from project.md when large | On demand, mid-session only |
| `archive/[name]/` | Stale project folders moved here instead of deleted | When pruning — folder-only users only |

---

## Common mistakes

**Loading too many files upfront.** Only upload or paste what's relevant. More context isn't always better — it can dilute the AI's focus.

**Forgetting to say "update memory hole."** If you don't do this, the session is lost. The AI's memory doesn't persist on its own — your files do.

**Not saving the updates.** The AI generates the updates, but you have to copy the output and save it back to your files manually. Nothing saves automatically.

**Using stale files.** If you edited files on another device and didn't sync first, you'll load outdated context. Always make sure you have the latest version before starting a session.