# Bobathon Feedback — Improvement Plan

## Overview

This plan consolidates feedback from Madison and Melissa's test sessions into
prioritized, categorized changes. Items are separated into **Must-Fix** (clarity
blockers, missing info, or errors that caused confusion) and **Nice-to-Have**
(suggestions that would improve flow or deepen the experience but aren't
blockers). Work is organized by the affected document/topic area.

---

## Section 1 — README.md

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| R1 | The term "diffs" in the Tips section ("Bob shows you diffs") is not defined; non-technical attendees did not know what it meant | Madison | Add a plain-language parenthetical: e.g. "diffs (a side-by-side view of what Bob is about to change)" |
| R2 | The safety/risk note appears *after* the permissions table; testers felt it should be read *before* they decided what to approve | Madison | Move the risk callout block so it appears before the permissions table, not below it |
| R3 | Contact name in the event-details table and footer is "Madison Ramsey" but should be "Melissa Hadley" | Madison | Replace all instances of "Madison Ramsey" and "madison.ramsey@ibm.com" with Melissa Hadley's name and email |
| R4 | After reading the README there is no clear "what to do next" instruction — testers didn't know to open a lab file or start a Bob chat | Madison | Add a visible "Start here →" call-to-action at the end of the Getting Started section: open Lab 1 instructions file, then open a Bob chat |

### Nice-to-Have (confirmed — all to be implemented)

| # | Issue | Source | Change |
|---|---|---|---|
| R5 | The README could briefly mention where to download the repo (HTTPS / Download ZIP) with a callout, since this confused at least one tester | Madison | In the "Getting started" section, add a one-sentence note before the numbered steps: "The lab files live in a Git repository — your setup guide walks you through cloning it in Step 5 of `resources/prereq-setup.md`." |
| R6 | The note about "open in Bob" / "open folder" / permissions dialog is implicit — not spelled out | Madison | In the "On the day" section, add a callout box before the numbered steps: "💡 If you're not sure how to open a folder in Bob or what 'Open in Bob' means, see Step 5 of your [pre-event setup guide](resources/prereq-setup.md)." |

---

## Section 2 — resources/prereq-setup.md (Setup Guide)

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| P1 | "Open in Bob" / opening the cloned folder is not obvious; testers didn't know what it meant and needed verbal help | Madison, Melissa | In Step 5, add a sub-step that explicitly says: after cloning, Bob will prompt "Open cloned repository?" — click Open. Then check the Explorer panel on the left for the lab folder. |
| P2 | After completing setup, there is no explicit redirect to start with the README — testers were unsure where to go next | Madison | Add a step at the very end of setup: "Step 6 — Read the README: open `README.md` in the Explorer and read it fully before starting Lab 1." |
| P3 | The permissions/security dialog for allowing Bob to access the folder is not mentioned — testers were surprised by it | Melissa | Add a note in Step 5 (or a new callout) saying Bob may ask for permission to read the workspace folder — click Allow. |

### Nice-to-Have (confirmed — all to be implemented)

| # | Issue | Source | Change |
|---|---|---|---|
| P4 | Could add a note that attendees must come to office hours — set the expectation that in-person setup assistance is crucial | Madison | Add a bold callout box at the top of the prereq-setup.md doc (right after the opening paragraph, before Step 1): "📅 **Come to office hours on September 21.** If anything in these steps doesn't work for you, don't wait until the day of the event. Office hours are specifically there to fix setup problems before the workshop." |

---

## Section 3 — Lab 1 (Personal Productivity) — instructions.md

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| L1-0a | No instruction in the lab on how to open the Bob chat panel — participants are expected to have already done this but it's never confirmed in the lab itself | New | Add a visible callout at the very top of the Setup section, before the checklist: "💬 **Open the Bob chat panel before you start.** Click the Bob icon in the left sidebar, or press `⌥ ⌘ B` (Mac) / `Ctrl + Alt + B` (Windows). You should see a text input at the bottom — that's where you'll type all your prompts throughout this lab." |
| L1-0b | No guidance to use a single conversation for the whole lab — this is critical because context carries across exercises only within the same conversation, and Badge Issuer Lite reviews the conversation history to evaluate badge eligibility | New | Add a second callout immediately after L1-0a in Setup: "💡 **Use one conversation for the entire lab — and keep it open until you claim your badge.** Start a new Bob chat now and keep it open through all three exercises. Bob holds your to-do list, your action items, and the full context of what you've done — but only within the same conversation. If you start a new chat, that context is gone and exercises that build on earlier ones won't work as intended. **There's a second reason too:** when you claim your badge at the end, Bob's Badge Issuer Lite mode reviews your conversation history to verify what you did. The richer and more complete that conversation, the smoother the badge evaluation." |
| L1-1 | The Setup checklist item about tone-reference-emails buries the "why" — testers didn't understand the purpose before being asked to add emails | Madison | Rewrite the optional checklist line to lead with the purpose: "Add 3–6 of your own past emails so Bob can match your writing tone when drafting email in Exercise 3." |
| L1-2 | There is no upfront disclaimer about not putting sensitive data into Bob before the email-upload instructions appear | Madison, Melissa | Add a visible callout/warning box at the top of the Setup section (before any exercise): "⚠️ Do not add confidential, sensitive, or customer data to any lab folder." |
| L1-3 | Exercise 1 tasks read like an overview/description rather than "do this now" step-by-step instructions; testers read to the end before feeling prompted to act | Melissa | Rewrite Exercise 1 task list to use explicit numbered step language: "Step 1: Type the following in the Bob chat interface…" instead of "Tell Bob about 3–4 things…" |
| L1-4 | "Tell Bob" / "Point Bob at" phrasing is unclear to non-technical attendees — they didn't know it meant typing in the chat | Madison, Melissa | Replace informal phrasing with explicit instruction: "In the Bob chat panel on the right side of the screen, type the following…" |
| L1-5 | Tool approval prompts ("There are tools that need to be approved") are not addressed in the lab instructions | Melissa | Add a note near the top of Exercise 1: "When Bob proposes an action, Approve and Reject buttons appear above the chat input — click Approve to continue, or refer to the README for auto-approve instructions. Note: if you only approve once, you will be prompted again for every subsequent action." |
| L1-6 | Exercise 1 ends abruptly; testers felt it was incomplete without being asked to view the final to-do list | Madison, Melissa | Add a closing step to Exercise 1: "Ask Bob to show you your updated to-do list" so participants can see the full result and Bob's recall/context before moving on. |
| L1-7 | Exercise 2: "Point Bob at sample-data/meeting-notes.md" — it was unclear if the exact path was required or just the intent | Madison | Add a parenthetical: "(You can type the path exactly or just say 'read the meeting notes file in the sample-data folder' — Bob will find it either way.)" |
| L1-8 | Exercise 3: How to add a file to the tone-reference-emails folder is not explained; testers tried drag-and-drop (which didn't work) and `.eml` / `.msg` files from Outlook (not supported) | Madison | Add a "How to add your emails" block in Exercise 3 or in the tone-reference-emails/README.md that explains: (a) create a new `.md` or `.txt` file in the folder, (b) paste email text in, (c) save. Include a note that `.eml` and `.msg` files from Outlook are not supported — paste the text instead. Add the prompt tip: "Have a different file type? Ask Bob to help you convert it to .md." |
| L1-9 | When toggling back and forth between the instructions file and the Bob chat, there's no guidance on how to keep both visible | Madison | Add a tip about navigation: "💡 Tip: Pin the instructions file in a tab so you can switch back to the chat easily." Or suggest keeping instructions open on the side. |

### Nice-to-Have (confirmed — all to be implemented)

| # | Issue | Source | Change |
|---|---|---|---|
| L1-N1 | Testers wanted insight into how the skills work in the background | Madison | After Exercise 2 and Exercise 3 respectively, add a collapsed "💡 Under the Hood" callout: for Exercise 2 explain that the `action-item-sync` skill powers the extraction and merging; for Exercise 3 explain that `tone-matched-drafting` reads the reference emails and shapes the draft. Point to `resources/bob-differentiators.md` for further reading. Keep each to 2–3 sentences — it should satisfy curiosity, not overwhelm. |
| L1-N2 | End-of-lab: ask Bob to show the full to-do list one more time to demonstrate cross-exercise context recall | Madison | Add a closing "🔄 Try This Before You Move On" step at the end of the lab (before Next Steps): ask Bob to show the complete updated to-do list including everything from all three exercises. Include a one-line observation prompt: "Notice that Bob remembers tasks you added in Exercise 1, items it extracted in Exercise 2, and any updates you made in Exercise 3 — all in a single conversation." |
| L1-N3 | Using real to-do items makes the value immediate and obvious | Melissa | In Exercise 1, promote the "use your own tasks" option to the *primary* path (put it first, before the sample prompt). Make the sample prompts a clearly-labelled fallback: "If you'd rather use examples, try these:" |
| L1-N4 | Tone reference: LinkedIn posts and prompted reply are good low-friction alternatives to finding old emails; no sensitive-data warning exists before people start adding content | Madison | **Three changes required:** (1) In Exercise 3 (instructions.md) and in `tone-reference-emails/README.md`, add a prominent ⚠️ sensitive-data warning **as the first thing participants read before any tone-reference instructions** — before the list of options, before any how-to steps. Wording: "⚠️ **Do not add confidential, sensitive, or customer data.** Only use content you'd be comfortable sharing in a shared lab environment. When in doubt, use Option 3 below — it requires no personal content at all." (2) Immediately after the warning, offer three clearly-labelled options for tone reference material: **Option 1** — 3–6 past emails you've written (paste as `.txt` or `.md`; `.eml` and `.msg` from Outlook are not supported); **Option 2** — 2–3 LinkedIn posts you've written (public, zero privacy risk); **Option 3** — a prompted reply: read `sample-incoming-email.md` in this folder, write a reply to it in a new `.txt` or `.md` file, and that reply becomes your tone sample. (3) Create `sample-data/tone-reference-emails/sample-incoming-email.md` with a realistic incoming email from a colleague asking for a project status update (different from the vendor thread context); warm but professional, 3–4 sentences, addressed to "Hi [Your Name]" so anyone can use it. Include brief instructions at the top of the file: "Read this email, then write your reply in a new file called `my-reply.md` in this same folder. Your reply becomes your tone reference." |
| L1-N5 | Exercise 2: explicit "show me the list" follow-up step | Madison | After the merge prompt in Exercise 2 Tasks, add a numbered step: "Ask Bob to show you your full updated to-do list." Include a sample prompt: `Show me my complete to-do list as it stands right now.` |

---

## Section 4 — Lab 2 (Research) — instructions.md

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| L2-0a | No instruction in the lab on how to open the Bob chat panel | New | Add the same "💬 Open the Bob chat panel" callout as L1-0a at the top of the Lab 2 Setup section. |
| L2-0b | No single-conversation guidance — Lab 2 builds on context within one thread, and Badge Issuer Lite reviews the conversation history to evaluate badge eligibility | New | Add a callout in Lab 2 Setup: "💡 **Use one conversation for this entire lab — and keep it open until you claim your badge.** Start a new Bob chat (or continue from Lab 1 if your facilitator advises it) and keep it open through all three exercises. Bob's ability to cross-reference multiple sources and remember your research question depends on holding the full context in one conversation. **Badge tip:** When you claim your badge at the end of the session, Bob's Badge Issuer Lite mode reads your conversation history to verify what you completed. The more you did and discussed in this conversation, the smoother that evaluation goes." |
| L2-1 | No upfront sensitive-data disclaimer (same issue as Lab 1) | Madison | Add the same ⚠️ sensitive-data warning callout at the top of the Setup section |
| L2-2 | "Point Bob at" phrasing appears again without definition | Madison | Same fix as L1-4 — explicit chat-panel instruction |
| L2-3 | Exercise 1 asks participants to point at source-a.md before they've read the research-brief.md — testers didn't understand the assignment before starting | Madison | Reorder Exercise 1 or add a step 0: "First, read `sample-data/research-brief.md` so you understand the question you're trying to answer before exploring the source documents." |
| L2-4 | "What is a curl command?" — the term appears without context (this may be from a prompt suggestion that includes curl; confirm location and clarify or remove) | Madison | Review all Exercise prompts for curl references and either remove them or add a plain-language note: "curl is a command-line tool for fetching web pages — Bob can run this for you automatically, no terminal knowledge needed." |

### Nice-to-Have (confirmed — all to be implemented)

| # | Issue | Source | Change |
|---|---|---|---|
| L2-N1 | After completing Lab 2 quickly (8 minutes straight-through), there's appetite to go deeper — encourage participants to research something real | Madison | Add a prominent **"🚀 Want more time with this?"** section at the end of the Exercises block (before Key Takeaways), with 3–4 specific stretch-exploration prompts that keep participants inside the lab's research frame. Examples: (a) "Bring a real question you're working on right now — paste in a document or URL and ask Bob to orient you in 60 seconds." (b) "Ask Bob to compare two of the source documents in a way the instructions didn't ask for." (c) "Ask Bob what questions the research *doesn't* answer — and why that matters." (d) "Ask Bob to role-play as a skeptical stakeholder and challenge the recommendation you just produced." Each stretch item should have 1-sentence framing, not just a raw prompt. |

---

## Section 5 — BADGE_GUIDE.md

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| B1 | Between Steps 2 and 3 there is no warning that Bob will ask for the event slug name and other details — testers were caught off guard | Madison | Add a note between Steps 2 and 3: "Bob will ask a few questions, including the event slug name. For this event the slug is: `it3_bobathon`." |
| B2 | It's unclear whether badging must be done in the same conversation thread as the labs | Madison | Add a callout: "You must claim your badge in a new Bob conversation after completing the labs. Bob will ask you to describe what you did — make sure you can summarize your lab work." (Or clarify if the same thread is required/preferred.) |
| B3 | The HTML certificate opens fine locally but not when pasted into a browser bar — participants couldn't find or open it | Madison | Clarify in Step 5 and the Tips section: "The HTML certificate is saved in the `badge-issuer-output/` folder in your workspace. To open it: in the Bob Explorer panel, right-click the file and select 'Reveal in File Explorer', then double-click to open in a browser." |

### Nice-to-Have (confirmed — all to be implemented)

| # | Issue | Source | Change |
|---|---|---|---|
| B-N1 | The more detail participants share about their work before claiming, the smoother the evaluation — this is in Tips but needs to be surfaced earlier and more actionably | Madison | Add a "📝 Before You Start" block at the very top of the Steps section (before Step 1): prompt participants to mentally prepare by recalling (a) which labs they completed, (b) one thing they learned or found surprising, (c) one specific example of something Bob did that saved them time. Phrase it as: "Take 30 seconds to think about this — you'll be asked." This sets them up for a smoother evaluation and a richer badge justification. |

---

## Section 6 — General / Cross-Cutting

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| G1 | No single upfront sensitive-data reminder exists that participants encounter before they start adding any content | Both | Confirm that the ⚠️ callout added to Lab 1 and Lab 2 setups (L1-2, L2-1) are consistent and visible — do not rely on only one location |
| G2 | The phrase "open in Bob" / "open folder" is never explained in any single place; it caused confusion at onboarding | Both | Ensure prereq-setup.md Step 5 (P1) and README Getting Started (R4) together give a complete, non-ambiguous explanation |
| G3 | Participants wanted to be explicitly encouraged to explore, ask questions, and not just follow the prompt scripts | Madison | Add a "Be curious" callout somewhere visible (end of README, or top of each lab): "The sample prompts are a starting point — feel free to ask Bob anything you're wondering about, including questions about how it works." |

### Nice-to-Have (confirmed — all to be implemented)

| # | Issue | Source | Change |
|---|---|---|---|
| G-N1 | At the end of Lab 1, participants had appetite for understanding how the skills work behind the scenes | Madison | In Lab 1 Additional Resources, promote the `bob-differentiators.md` link from a bullet in a list to a standalone callout box with a 1-sentence hook: "Curious how Bob knew to extract action items or write in your tone? Read this →". In Lab 2, do the same at the end, framed around MCP and multi-source synthesis. |
| G-N2 | Event timing: 1h15m total for setup + Lab 1 + Lab 2 twice | Madison | No content change needed — note in event debrief documentation only. |
| G-N3 | "Be curious / explore freely" — implement throughout each lab at the point of relevance, not just at the end | Madison | **This is the highest-priority nice-to-have.** Exploration prompts must be embedded **inline within each exercise**, immediately after the core tasks and before the Expected Outcome — while participants are still engaged with that specific capability. Do NOT move them to the end of the lab. Additionally, add a single short "🧭 Keep Exploring" closing section after the last exercise as a capstone that ties it together. Design for each inline callout: (a) a brief framing sentence ("If you have a few extra minutes, try this…"), (b) 2–3 "what if" questions each with a ready-to-copy prompt, (c) no more than one short paragraph — it must not look like required work. The closing section is longer (4–5 prompts) and frames the full lab as a sandbox, not a checklist. See per-exercise breakdown below. |

**Lab 1 — Inline "🧭 Want to explore?" per exercise:**

*After Exercise 1 (To-Do List):*
- "What if I asked Bob to group my tasks by category instead of priority?" → `Reorganize my to-do list grouped by type of work instead of priority order.`
- "What if I asked Bob to draft a calendar hold for one of my tasks?" → `Based on my to-do list, draft a calendar hold email for the Thursday planning session.`
- "What if I asked Bob how it's tracking the list internally?" → `How are you keeping track of my to-do list — are you saving it somewhere or holding it in the conversation?`

*After Exercise 2 (Action Item Extraction):*
- "What if Bob summarized my whole day in one sentence from everything it's read?" → `Based on the meeting notes and email thread, summarize the one most important thing I need to do today.`
- "What if I asked Bob to flag risks or follow-up questions I might have missed?" → `Based on the email thread, what questions should I be asking that I haven't yet?`
- "What if I asked Bob to draft a status update email to my manager based on the action items?" → `Draft a short status update email to my manager summarizing what I'm working on this week, based on the action items you extracted.`

*After Exercise 3 (Email Drafting):*
- "What if I asked Bob to try a completely different tone — more casual?" → `Rewrite the email draft but make it more casual — I'm on good terms with this vendor.`
- "What if I asked Bob to make the email shorter and more direct?" → `Cut this draft down to 3 sentences. Keep only the ask.`
- "What if I asked Bob what it noticed about my writing style from the reference emails?" → `Based on the emails I shared, describe how I typically write — tone, formality, sentence style.`

*Closing "🧭 Keep Exploring" section (after Exercise 3, before Key Takeaways):*
- Framing: "You've covered the core of this lab. Bob can go further — here are some things worth trying if you still have time."
- "Bring something real: paste in an actual email you need to respond to right now and ask Bob to draft a reply in your tone."
- "Ask Bob what it would do differently: `Looking at the to-do list and the action items you extracted, what would you do differently if you were managing my day?`"
- "Test Bob's memory: `Without looking back, summarize everything we've worked on since the start of this conversation.`"

---

**Lab 2 — Inline "🧭 Want to explore?" per exercise:**

*After Exercise 1 (Getting Up to Speed):*
- "What if I asked follow-up questions Bob didn't anticipate?" → `What's the most controversial or contested claim in this document?`
- "What if I asked Bob to explain it like I'm completely new to this field?" → `Explain the key points from source-a.md as if I've never worked in this industry before.`
- "What if I brought in a real document from my own work?" → `[Paste or point Bob at a document you're currently working with.] Give me a plain-language overview and tell me what I most need to understand.`

*After Exercise 2 (Multi-Source Synthesis):*
- "What if I asked Bob to steelman the opposing view?" → `Based on the sources, argue the strongest case against the conclusion we just reached.`
- "What if I asked Bob to identify the single most critical unknown?" → `What is the most important piece of information missing from these three sources that would change the recommendation?`
- "What if I asked Bob to identify where the sources might be biased?" → `Are any of these sources one-sided or missing a perspective? Flag anything that reads like advocacy rather than balanced analysis.`

*After Exercise 3 (Structured Deliverable):*
- "What if I changed the audience entirely?" → `Rewrite this briefing for an audience of front-line managers instead of senior leaders. Change what you emphasize.`
- "What if I asked Bob to identify the weakest part of the recommendation?" → `What's the most likely objection a skeptical reader would raise to this recommendation, and how would you respond to it?`
- "What if I pushed Bob to make the deliverable shorter?" → `Cut this to half the length. Keep only what changes the reader's thinking or action.`

*Closing "🧭 Keep Exploring" section (after Exercise 3, before Key Takeaways):*
- Framing: "Still have time? The best research conversations go beyond the brief. Try one of these."
- "Bring real work: swap in a document or question from something you're actually working on right now."
- "Ask Bob what it would prioritize: `If you had to pick one finding from this research to act on immediately, what would it be and why?`"
- "Test the limits: ask Bob something the sources don't cover and see how it handles the gap."

---

## Section 7 — Lab 3 (Developer Efficiency) — instructions.md

### Must-Fix

| # | Issue | Source | Change |
|---|---|---|---|
| L3-0a | No instruction in the lab on how to open the Bob chat panel — same gap as Labs 1 and 2 | New | Add the same "💬 **Open the Bob chat panel before you start.**" callout at the top of Setup, before the checklist. Same wording as L1-0a. |
| L3-0b | No explicit single-conversation guidance — in a 90-minute lab with 7 checkpoints this is especially important; context compounds across checkpoints, and Badge Issuer Lite reviews the full conversation history to evaluate badge eligibility | New | Add a callout immediately after L3-0a in Setup: "💡 **Use one conversation for the entire lab — and keep it open until you claim your badge.** Start a new Bob chat now and keep it open through all seven checkpoints. Bob builds cumulative context as you work — the codebase orientation from Checkpoint 1 informs the debugging in Checkpoint 4, and the full picture is what makes Checkpoints 6 and 7 most powerful. If you start a new chat mid-lab, that context resets. **Badge tip:** When you claim your Bobathon badge at the end, Bob's Badge Issuer Lite mode switches into a special evaluation mode and reads your conversation history to verify what you completed. The more checkpoints you worked through in this conversation — and the more you explored and discussed — the smoother and more accurate that evaluation will be. Keep this chat open all the way through." |
| L3-1 | Contact name "Madison Ramsey" appears on line 8 (header) and line 369 (Next Steps) — should be Melissa Hadley | New | Replace both instances of "Madison Ramsey" and "madison.ramsey@ibm.com" with Melissa Hadley's name and email. Same fix as R3 in README. |
| L3-2 | Repository overview diagram in Setup is incomplete — lists only `test_transform.py` and `test_validate.py` but the actual `tests/` folder contains four files: `test_ingest.py`, `test_risk_scorer.py`, `test_transform.py`, and `test_validate.py` | New | Update the repo tree diagram to include all four test files so participants aren't confused when Bob references a test file not shown in the overview. |
| L3-3 | No sensitive-data note — the codebase contains a deliberately planted hardcoded credential (`B0nk@Pipeline2024!` in `config/settings.py`); participants need to know this is intentional sample data, not something to copy or report as a real security issue | New | Add a targeted note in Setup (not a generic warning — specific to this lab): "🔐 **Note on the planted credential:** This codebase contains a deliberately hardcoded password in `config/settings.py`. You will find it in Checkpoint 3 — this is intentional sample data for the security scan exercise. Do not use this pattern in real code, and do not treat it as a live secret." |

### Nice-to-Have (confirmed — all to be implemented)

| # | Issue | Source | Change |
|---|---|---|---|
| L3-N1 | No inline "explore further" prompts per checkpoint — the opening callout is good but there are no "what if" prompts after each checkpoint to extend engagement in context | New (G-N3 equivalent) | Add a "🧭 Want to go deeper?" inline callout after each checkpoint, with 2–3 developer-flavoured "what if" prompts tied specifically to what was just done. See per-checkpoint breakdown below. |
| L3-N2 | No `bob-differentiators.md` link or further-reading callout at the close of Lab 3 | New (G-N1 equivalent) | Add a standalone callout at the end of the lab (before or after Reflection), framed for developers: "Curious how Bob does this at scale? Read about Bob Findings, sub-task orchestration, and enterprise modernization →" linking to `resources/bob-differentiators.md`. |

**Lab 3 — Inline "🧭 Want to go deeper?" per checkpoint:**

*After Checkpoint 1 (Orient in the Codebase):*
- "What if I asked Bob to draw the data flow as a sequence of steps?" → `Describe the end-to-end data flow of this pipeline as a numbered sequence of steps, from raw CSV to data warehouse.`
- "What if I asked Bob which module is most likely to break in production?" → `Based on what you've seen, which module in this pipeline is most fragile or most likely to cause a production incident? Why?`
- "What if I asked Bob what's missing from this project entirely?" → `What would a production-ready version of this pipeline need that this codebase doesn't have yet?`

*After Checkpoint 2 (Read and Explain Code):*
- "What if I asked Bob to explain it like I'm a junior developer?" → `Explain the normalize_amounts function in pipeline/transform.py as if I've never seen pandas before.`
- "What if I asked Bob to identify the most complex function in the codebase?" → `Which function in this codebase is the hardest to understand at a glance, and why?`
- "What if I asked Bob to spot any functions that do too many things at once?" → `Are there any functions in this codebase that violate the single-responsibility principle? Show me the worst offender.`

*After Checkpoint 3 (Search and Pattern Recognition):*
- "What if I asked Bob to find all the places where errors are silently swallowed?" → `Find all places in this codebase where exceptions are caught but not logged or re-raised. List them.`
- "What if I asked Bob to suggest how to fix the hardcoded credential properly?" → `How should the hardcoded password in config/settings.py be managed instead? Show me the recommended pattern using environment variables and a secrets manager.`
- "What if I asked Bob what else might be a security risk beyond what it already found?" → `Beyond the hardcoded credential, are there any other security concerns in this codebase I should be aware of?`

*After Checkpoint 4 (Debug and Troubleshoot):*
- "What if I asked Bob to find other places where the same class of bug might exist?" → `Are there other functions in this codebase that could produce silent NaN or division-by-zero issues under similar conditions? Scan for them.`
- "What if I asked Bob to explain the fix in terms a non-developer stakeholder could understand?" → `Explain the bug we just fixed and why it matters in plain English — no code, no jargon.`
- "What if I ran all the tests, not just the ones for transform?" → `Run the full test suite with pytest and show me a summary of all results.`

*After Checkpoint 5 (Make and Validate Code Changes):*
- "What if I asked Bob to review the code I just added for quality?" → `Review the add_weekend_flag function and its test for code quality. What would you change or improve?`
- "What if I asked Bob whether this change could break anything else?" → `Does adding add_weekend_flag to run_transformations have any downstream effects on loader.py or the risk scorer?`
- "What if I asked Bob to add a docstring to my new function?" → `Add a complete docstring to add_weekend_flag in pipeline/transform.py.`

*After Checkpoint 6 (Bob Findings):*
- "What if I asked Bob to prioritize all the findings it surfaced?" → `Of all the Findings you surfaced in the ML code, which one would you fix first if this were going to production tomorrow? Why?`
- "What if I asked Bob how the caching fix we applied changes the performance profile?" → `Now that we've added module-level model caching, how does the memory and startup-time profile of risk_scorer.py change?`
- "What if I asked Bob to apply one more finding end-to-end?" → Pick any remaining finding and ask Bob to explain, implement, and test the fix.

*After Checkpoint 7 (Build Something New):*
- "What if I asked Bob where in the pipeline ReportGenerator should actually be called?" → `Where in the existing pipeline flow should ReportGenerator be invoked? Show me how to wire it in.`
- "What if I asked Bob what a v2 of ReportGenerator would look like?" → `If we were to build a more sophisticated version of ReportGenerator — charts, export formats, configurable metrics — what would the design look like?`
- "What if I asked Bob to reflect on the whole session?" → `Looking at everything we've done across all checkpoints, where did you save me the most time and where did I have to do the most work myself?`

---

## Status

> ✅ **Implementation complete.**
> Event slug: `it3_bobathon` · Contact: Melissa Hadley

### Section 1 — README.md
- [x] R1 — "diffs" defined with plain-language parenthetical
- [x] R2 — risk/safety note moved above permissions table
- [x] R3 — contact updated to Melissa Hadley throughout
- [x] R4 — "Start here →" CTA added after Getting Started steps
- [x] R5 — repo/Git clone note added in Before the Event section
- [x] R6 — "Open in Bob" callout added in On the Day section

### Section 2 — resources/prereq-setup.md
- [x] P1 — Step 5 expanded: "Open cloned repository?" prompt explained, Explorer confirmation added
- [x] P2 — Step 6 added: redirect to README then Lab 1
- [x] P3 — Permission dialog (Allow/Yes) noted in Step 5
- [x] P4 — Office hours callout added at top of document

### Section 3 — Lab 1 instructions.md
- [x] L1-0a — Chat panel open instruction added to Setup
- [x] L1-0b — Single-conversation callout added to Setup
- [x] L1-0b (badge) — 🏅 badge evidence callout added as separate block
- [x] L1-1 — Tone-reference checklist item rewritten to lead with purpose
- [x] L1-2 — Sensitive-data warning added to Setup
- [x] L1-3 — Exercise 1 rewritten as explicit numbered Steps
- [x] L1-4 — "Tell Bob" / "Point Bob at" replaced with "In the Bob chat panel, type…"
- [x] L1-5 — Tool approval note added at top of Exercise 1
- [x] L1-6 — "Show me my current to-do list" closing Step 4 added to Exercise 1
- [x] L1-7 — Path flexibility note added to Exercise 2 Step 1
- [x] L1-8 — How-to-add-files block + Outlook format note + Option 1/2/3 added to Exercise 3
- [x] L1-9 — Tab pinning tip added to Setup
- [x] L1-N1 — "Under the Hood" callouts added after Exercise 2 and Exercise 3
- [x] L1-N2 — "🔄 Try This Before You Move On" section added before Key Takeaways
- [x] L1-N3 — Exercise 1 real-tasks-first framing promoted to primary path
- [x] L1-N4 — Three tone-reference options (emails / LinkedIn / prompted reply) + sensitive-data warning first; sample-incoming-email.md created
- [x] L1-N5 — "Show me my complete to-do list" Step 4 added to Exercise 2

### Lab 1 — tone-reference-emails/README.md
- [x] Full rewrite: sensitive-data warning first, three labelled options, file-adding instructions, Outlook note

### Lab 1 — sample-data/tone-reference-emails/sample-incoming-email.md
- [x] New file created: realistic status-update incoming email from colleague Jamie, with Option 3 instructions

### Section 4 — Lab 2 instructions.md
- [x] L2-0a — Chat panel open instruction added to Setup
- [x] L2-0b — Single-conversation + badge evidence callouts added to Setup
- [x] L2-1 — Sensitive-data warning added to Setup
- [x] L2-2 — "Point Bob at" replaced with "In the Bob chat panel, type…" throughout
- [x] L2-3 — Step 0 (read research-brief.md first) added to Exercise 1
- [x] L2-4 — No curl references found in Lab 2 prompts; confirmed no change needed
- [x] L2-N1 — 🧭 Want to explore? inline prompts added after each exercise
- [x] G-N3 — 🧭 Keep Exploring closing section added
- [x] "Optional" label added to "use your own content" callout

### Section 5 — BADGE_GUIDE.md
- [x] B1 — Event slug `it3_bobathon` added between Steps 2 and 3
- [x] B2 — "Stay in the same conversation" callout added at very top of file and within Step 2
- [x] B3 — HTML certificate opening instructions added in Step 5 and Tips
- [x] B-N1 — "📝 Before You Start" prep block added before Steps

### Section 6 — Cross-Cutting
- [x] G1 — Sensitive-data warning consistent across Lab 1 and Lab 2 Setup sections
- [x] G2 — "Open in Bob" explained in prereq-setup.md Step 5 and README On the Day section
- [x] G3 — "Be curious" framing embedded in each lab's 🧭 Keep Exploring section
- [x] G-N1 — bob-differentiators.md promoted to standalone callout in Lab 1 (Under the Hood) and Lab 3 (end-of-lab callout); Lab 2 already references it in Key Takeaways
- [x] G-N3 — Inline 🧭 explore prompts added per exercise in Lab 1 and Lab 2; plus closing Keep Exploring sections

### Section 7 — Lab 3 instructions.md
- [x] L3-0a — Chat panel open instruction added to Setup
- [x] L3-0b — Single-conversation + badge evidence callouts added to Setup (strongest version, 7-checkpoint framing)
- [x] L3-1 — Contact updated to Melissa Hadley (header line 8 and Next Steps line)
- [x] L3-2 — Repo tree diagram updated to include all four test files (test_ingest.py, test_risk_scorer.py, test_transform.py, test_validate.py)
- [x] L3-3 — Planted credential note added to Setup
- [x] L3-N1 — 🧭 Want to go deeper? inline callouts added after all 7 checkpoints
- [x] L3-N2 — bob-differentiators.md standalone callout added before Reflection section

### Post-implementation fixes
- [x] BADGE_GUIDE.md — "Stay in the same conversation" callout moved to very top of file (before Prerequisites)
- [x] Lab 2 — "use your own content" callout labelled as Optional
