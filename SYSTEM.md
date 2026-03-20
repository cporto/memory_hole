# Memory Hole — How the System Works

This file explains the logic behind how Memory Hole captures decisions, triggers updates, and keeps your memory clean. Load it if you want to understand what's happening under the hood — you don't need it for daily use.

---

## The update trigger

When you say **"update memory hole"** at the end of a session, the AI generates complete, ready-to-paste replacement blocks for every file that changed. You copy the output and save it back to your files manually. Nothing saves automatically.

Every update captures:
- What changed and why
- Any decisions made — with the reasoning, not just the outcome
- New open questions
- What was resolved

### Update output rules

- Before each block, announce which file it belongs to and where to save it. Example: "This goes into `projects/my-project/project.md` in your private repo." Never drop a block without that context.
- Only files where content, state, or decisions actually changed get output — untouched files are left alone
- Every decision must include: Decision, Why, Rejected alternatives, Why rejected
- Decisions are captured in the exact terms they were made — no compressing or reframing
- "Current state" and "Next action" always reflect end-of-session state, not mid-session
- Open questions: `[ ]` new, `[x]` resolved, `[~]` partial
- If something was discussed but not decided, it becomes a new open question — it doesn't disappear
- Date format: `YYYY-MM-DD HH:MM [local timezone]` always
- Output is dense, not verbose. Structured data, not prose. Every line is signal.
- No preamble, no summary paragraphs, no commentary. Just the blocks.

---

## Event-based update trigger

The AI doesn't wait for you to say "update memory hole" to notice that something important happened. It watches for qualifying decisions and captures them automatically.

### What qualifies as a decision

A qualifying decision meets one or more of these:

- **Architectural** — affects how something is built or structured
- **Directional** — rules out an approach for a stated reason
- **Rule-setting** — creates a constraint that governs future behavior

Provisional statements do not qualify. "Let's try X" or "maybe X" are not decisions.

### Collection window

One exchange = one user message + one AI response.

When a qualifying decision lands:
1. Don't trigger immediately — open a 2-exchange collection window
2. For each subsequent exchange, check: did another qualifying decision land?
   - Yes → absorb it, reset the window to 2 exchanges, continue
   - No → decrement the window by 1
3. When the window reaches 0, trigger the update automatically
4. Output the full update blocks for all collected decisions, then notify the user
5. Close the window and reset — ready to open again on the next qualifying decision

### Before auto-triggering

The AI announces what it's capturing before running a mid-session update:

> *"Capturing [brief description] before we move on — I'll include this in the full update at session end."*

Mid-session captures are assists, not replacements. You still own the end-of-session trigger.

### Periodic check-in

Every 10 exchanges, the AI checks in:

> *"Poking my head in — anything worth saving from the last few exchanges?"*

If you confirm something landed, it's treated as a qualifying decision and the update triggers immediately. If not, the counter resets and the conversation continues.

---

## Context warnings

The AI tracks context usage and warns you before things get tight.

- **60% context used** — warning issued. Example: *"Heads up — we're at 60% context. Might be time to think about saving your work before I start getting weird."*
- **80% context used** — update triggers automatically without being asked. The full update blocks are output immediately, then the user is notified. Example: *"We're at 80% context — this is your last clean exit. Here's your update, ready to copy."*

---

## All triggers use the same format

Whether fired by a decision cluster, a periodic check-in, a context warning, or manually — the output is always the same: full replacement blocks, ready to paste.
