# Session 2 Feedback — Improvement Plan

## Overview

This plan consolidates feedback from Madison (session 2) and Brandy Guillory into
prioritized, categorized changes. Two themes: (1) the event/repo title needs updating
to reflect the official Truist-given session name, and (2) several setup-friction
points were identified that testers hit before even reaching the labs.

Work is organized by the affected document/topic area.

---

## Section 1 — Title / Branding Update (All Relevant Files)

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| T1 | The event title used throughout the repo is "IT^3 Bob-a-thon" or "Women in Technology Bob-a-thon"; Truist has named the session **"IBM Workshop"** | Madison | Update the GitHub repo title and all prominent heading references to: **"WIT IT^3 Conference: IBM Workshop — Bob-a-thon"** |
| T2 | README line 1 heading reads `# IT^3 Bob-a-thon — Participant Guide` | Madison | Update to `# WIT IT^3 Conference: IBM Workshop — Bob-a-thon` |
| T3 | README line 4 reads "Welcome to the Women in Technology Bob-a-thon!" | Madison | Update welcome sentence to reflect new official title |
| T4 | `resources/prereq-setup.md` line 1 heading and line 267 footer both say "IT^3 Bob-a-thon" | Madison | Update both to new title |
| T5 | `resources/external-links.md` heading and footer say "IT^3 Bob-a-thon" | Madison | Update both to new title |
| T6 | `Lab 3 - Developer Efficiency/instructions.md` sub-heading line 2 says "IT^3 Bob-a-thon" | Madison | Update to new title |
| T7 | `Lab 3 - Developer Efficiency/data-pipeline/README.md` line 3 references "IT^3 Bob-a-thon" | Madison | Update to new title |

**Affected files summary:**
- `README.md` (lines 1, 4)
- `resources/prereq-setup.md` (lines 1, 267)
- `resources/external-links.md` (lines 1, 90)
- `Lab 3 - Developer Efficiency/instructions.md` (line 2)
- `Lab 3 - Developer Efficiency/data-pipeline/README.md` (line 3)

---

## Section 2 — README: IBM Bob Overview Block

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| B1 | The README jumps straight into event details with no explanation of what IBM Bob or a Bob-a-thon actually is — first-time participants have no context | Madison | Add an **"About this workshop"** block in `README.md` **after the event details table and its closing `---` divider, and before the "What you'll need" section**. Content: two short paragraphs — "What is IBM Bob?" and "What is a Bob-a-thon?" — using the approved wording supplied by Madison, lightly refined for clarity (see Content block below). |

**Content to add (refined from Madison's wording):**

> ## 🤖 About this workshop
>
> ### What is IBM Bob?
> IBM Bob is an AI-powered assistant built into your development environment. It helps engineers and non-technical teammates alike get work done faster — answering questions, automating daily tasks, and writing, fixing, or refactoring code — all through a simple chat interface. You don't need to know how to code to get value from it.
>
> ### What is a Bob-a-thon?
> A Bob-a-thon is a hands-on learning experience where you work through guided exercises to explore how AI can support research, productivity, and software development tasks. Think of today's labs as a low-stakes sandbox: the goal is to get comfortable asking Bob for help and to leave with a feel for what it can do in your day-to-day work.

---

## Section 3 — Setup Guide: New Folder Creation + Repo Cloning UX

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| S1 | Participants didn't know to click "New Folder" or where to store files; they needed to know to create a folder like `boblabs` in `/Documents` and then use "Select as repository destination" | Brandy | In `resources/prereq-setup.md` Step 5 (cloning the repo), add a sub-step before the clone action: "Create a destination folder first: open your file browser, navigate to `/Documents`, and create a new folder called `boblabs`. When Bob asks where to clone the repository, choose this folder using **Select as repository destination**." |
| S2 | After cloning, participants may be prompted to "Trust the Authors" — this was not mentioned anywhere and surprised users | Brandy | Add a note in Step 5 (after the clone action): "After cloning, Bob or your system may ask **'Do you trust the authors of this folder?'** — click **Trust** (or Yes). Without this, Bob cannot read the files in the workspace." |
| S3 | After cloning, Bob may show an update prompt — participants didn't know to skip it | Brandy | Add a note immediately after S2: "You may also see a prompt to install an update — click **Skip** (or close the dialog). You do not need to update Bob before the lab." |
| S4 | The folder/file explorer requires a hard double-click to expand, and there may be a noticeable delay — participants were confused by the lag | Brandy | Add a tip callout in Step 5: "💡 **Double-click** to expand folders in the Explorer panel. There may be a short delay — wait a moment before clicking again." |

---

## Section 4 — Lab 1: VM Clipboard / Multi-Line Prompt Warning

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| V1 | In a VM environment, if participants don't use clipboard sync and instead use "Send Text" to paste the Exercise 1 prompt, the multi-sentence prompt is sent one line at a time — Bob executes each sentence as a separate command, causing confusion | Brandy | In `Lab 1 - Productivity/instructions.md` Setup section, add a VM-specific warning callout: "⚠️ **If you're working in a TechZone VM:** Do not use 'Send Text' to enter the Exercise 1 prompts — it sends each sentence separately and will confuse Bob. Instead, use **clipboard sync**: copy the entire prompt on your local machine, enable clipboard sync in the VM settings, then paste (`Ctrl+V`) into the Bob chat." |

---

## Section 5 — All Labs: Auto-Approve Todo Tools

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| A1 | Participants were repeatedly prompted to approve tool actions (specifically todo/subtask tools) and didn't know to approve all at once | Brandy, Melissa | In each lab's Setup section (Lab 1, Lab 2, Lab 3), add a step or callout: "💡 **Approve all todo tools for the task.** When Bob first proposes using a tool (like the to-do manager), you'll see Approve/Reject buttons. Click **Approve** and select **Approve All for this Task** (or the equivalent all-at-once option) so you're not prompted again for every subsequent step in the same task. If you only approve once individually, you will be prompted again for each action." |

---

## Status

> ✅ **Implementation complete.**
> New feedback from Madison (session 2) and Brandy Guillory — fully implemented.

### Section 1 — Title/Branding
- [x] T1–T7 — Updated title in all 5 affected files to "WIT IT^3 Conference: IBM Workshop — Bob-a-thon"

### Section 2 — README IBM Bob Overview Block
- [x] B1 — "About this workshop" block added to README.md (after event details, before "What you'll need")

### Section 3 — Setup Guide: Folder / Clone UX
- [x] S1 — "Create boblabs folder in Documents → Select as Repository Destination" added to Step 4
- [x] S2 — "Trust the Authors" prompt note added as Step 7
- [x] S3 — "Skip update" prompt note added as Step 8
- [x] S4 — Double-click / delay tip added as callout in Step 8

### Section 4 — Lab 1 VM Clipboard Warning
- [x] V1 — VM clipboard sync warning added to Lab 1 Setup (after chat panel callout)

### Section 5 — All Labs Auto-Approve Todo Tools
- [x] A1 — "Approve All for this Task" callout added to Lab 1, Lab 2, and Lab 3 Setup sections
