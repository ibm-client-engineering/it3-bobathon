# Lab 1: Personal Productivity

**Duration:** 30 minutes
**Difficulty:** Beginner
**Prerequisites:** Bob installed and running

## 🎯 Objectives

By the end of this lab, you will be able to:
- Have Bob create and maintain a running to-do list conversationally
- Extract action items from a meeting transcript and an email thread
- Synthesize action items from multiple sources into one prioritized task list
- (Optional) Personalize Bob's writing style to match your own tone using reference emails
- Draft a follow-up email faster using AI assistance

## 📋 Setup

> 💬 **Open the Bob chat panel before you start.** Click the Bob icon in the left sidebar, or press `⌥ ⌘ B` (Mac) / `Ctrl + Alt + B` (Windows). You should see a text input at the bottom — that's where you'll type all your prompts throughout this lab.

> 💡 **Use one conversation for the entire lab — and keep it open until you claim your badge.**
> Start a new Bob chat now and keep it open through all three exercises. Bob holds your to-do list, your action items, and the full context of what you've done — but only within the same conversation. If you start a new chat mid-lab, that context is gone and exercises that build on earlier ones won't work as intended.

> 🏅 **Important — this conversation is your badge evidence.** When you finish the lab and claim your Bobathon badge, Bob's Badge Issuer Lite mode stays in this same chat and reads your conversation history to verify what you completed. **Do not close or start a new chat before claiming your badge.** The richer your conversation — the more you explored, asked, and tried — the smoother and faster that evaluation will be.

> ⚠️ **Do not add confidential, sensitive, or customer data to any lab folder.** Only use content you're comfortable sharing in a shared lab environment.

> 📌 **Tip:** Keep this instructions file open in a pinned tab so you can switch back to the Bob chat easily. In Bob, right-click the tab and select **Keep Open** (or **Pin Tab**) to prevent it from closing automatically.

Before starting, ensure you have:
- [ ] Bob running with the chat panel open (see above)
- [ ] Access to the sample data in `Lab 1 - Productivity/sample-data/` (provided in this lab folder)
- [ ] **Optional:** Tone reference material saved in `Lab 1 - Productivity/sample-data/tone-reference-emails/` so Bob can match your writing style when drafting email in Exercise 3. See that folder's `README.md` for the three options available — including a zero-effort option that requires no personal content. If you skip this, Bob will use a neutral professional tone instead.

> **💡 Custom skills power this lab.** Exercises 2 and 3 are backed by two custom Bob skills (`action-item-sync` and `tone-matched-drafting`). Bob applies them automatically based on what you ask it to do, no slash command needed.

> **🔄 Use your own content instead of the samples.** Every exercise below uses sample files (`meeting-notes.md`, `email-chain.md`, `tone-reference-emails/`) so the lab works out of the box. If you'd rather use the real thing, just give Bob your own meeting transcript, email chain, or past emails instead, either by pasting the content directly into the chat or by pointing Bob to your own file(s) in place of the sample path. Nothing else about the exercise changes.

## 🔨 Exercises

### Exercise 1: A To-Do List Bob Maintains For You (10 minutes)

**Scenario:** You have a handful of tasks on your mind. Instead of writing them down yourself, have Bob track them for you, and keep the list updated as things change.

> 🔧 **When Bob proposes an action**, Approve and Reject buttons appear above the chat input — click **Approve** to continue. If you only approve once, you'll be prompted again for each subsequent action. To approve all actions automatically, enable **Read**, **Edit**, and **Execute** in the Auto-Approve toolbar above the chat input (see the README for details).

**Step 1:** In the Bob chat panel on the right side of the screen, start with your own real tasks if you have some — it makes the value obvious immediately. Type something like:

```
I need to get a few things done today: [list your own tasks here]. Please track these for me as a to-do list.
```

**If you'd rather use examples, try this instead:**
```
I need to get a few things done today:
- Send the budget summary to my manager
- Follow up with the vendor about the invoice discrepancy
- Book a conference room for Thursday's planning session

Please track these for me as a to-do list.
```

**Step 2:** In the Bob chat panel, mark one item complete:
```
I finished the budget summary; mark that one done.
```

**Step 3:** Add a new task and reprioritize:
```
Add "review Q3 numbers before Thursday's meeting" and make it the top priority.
```

**Step 4:** Ask Bob to show you the updated list:
```
Show me my current to-do list.
```

**Expected Outcome:**
- Bob maintains a live, structured task list throughout the conversation
- You can update, complete, and reprioritize items just by talking to Bob
- You never had to open a separate notes app or spreadsheet

> 🧭 **Want to explore?** If you have a few extra minutes, try one of these:
> - "What if Bob grouped my tasks by type of work instead of priority?" → `Reorganize my to-do list grouped by category instead of priority order.`
> - "What if I asked Bob to draft a calendar hold for one of my tasks?" → `Based on my to-do list, draft a calendar hold email for the Thursday planning session.`
> - "What if I asked Bob how it's tracking the list?" → `How are you keeping track of my to-do list — are you saving it somewhere or holding it in the conversation?`

**💡 Real-time Value Indicator:**
This is the same underlying capability Bob uses to track its own multi-step work, applied here to *your* day. No formatting, no separate app, no manual reordering.

---

### Exercise 2: Turning Meeting Notes and Emails Into Action Items (10–15 minutes)

**Scenario:** Action items are scattered across your meeting notes and a follow-up email thread. Instead of re-reading both and writing your own list, have Bob do the extraction, and merge the results into the to-do list from Exercise 1.

> **Use your own content (optional):** You can swap in your own real meeting notes and/or email thread instead of the samples below (paste them in, or point Bob to your own file). Using the provided samples works just as well if you'd rather not.

**Step 1:** In the Bob chat panel, type the following (you can use the exact path or describe the file — Bob will find it either way):
```
Read sample-data/meeting-notes.md and list the action items, who owns each one, and any deadlines mentioned.
```

**Step 2:** In the Bob chat panel, do the same for the email thread:
```
Now read sample-data/email-chain.md and do the same thing.
```

**Step 3:** Merge both sets into your running to-do list:
```
Merge the action items from both into my to-do list from before. Only include the ones that are actually mine to do, and flag anything with an unclear owner.
```

**Step 4:** Ask Bob to show you the full updated list:
```
Show me my complete to-do list as it stands right now.
```

**Expected Outcome:**
- Bob accurately extracts action items, owners, and deadlines from unstructured notes and emails
- Duplicate or overlapping items from the two sources are consolidated
- Your to-do list now reflects real commitments from a meeting and an email thread, not just what you remembered

**💡 Real-time Value Indicator:**
Manually re-reading meeting notes and an email thread to build a task list typically takes 10–15 minutes and things get missed. Bob does the extraction in seconds and catches items you'd likely have missed on a first read.

> 💡 **Under the Hood:** This exercise uses the `action-item-sync` skill — a custom Bob skill that knows how to extract owners, deadlines, and action items from unstructured text and merge them without duplicating. Bob applied it automatically based on what you asked. Curious how custom skills work? See [`resources/bob-differentiators.md`](../resources/bob-differentiators.md).

> 🧭 **Want to explore?** If you have a few extra minutes:
> - "What if Bob summarized my whole day in one sentence?" → `Based on the meeting notes and email thread, summarize the single most important thing I need to do today.`
> - "What if I asked Bob what questions I should still be asking?" → `Based on the email thread, what questions should I be asking that I haven't yet?`
> - "What if I asked Bob to draft a status update to my manager?" → `Draft a short status update email to my manager summarizing what I'm working on this week, based on the action items you extracted.`

---

### Exercise 3 (Optional): Drafting Email in Your Own Voice (10 minutes)

**Scenario:** You need to send a follow-up email, but you want it to sound like *you* wrote it, not like generic AI output.

**Before you start — choose your tone reference option:**

> ⚠️ **Do not add confidential, sensitive, or customer data.** Only use content you'd be comfortable sharing in a shared lab environment. When in doubt, use Option 3 below — it requires no personal content at all.

- **Option 1 — Past emails you've written:** Paste 3–6 emails as `.txt` or `.md` files into `sample-data/tone-reference-emails/`. Note: `.eml` and `.msg` files from Outlook are not supported — copy and paste the text instead. Have a different file type? Ask Bob: `Help me convert this file to .md format.`
- **Option 2 — LinkedIn posts you've written:** Paste 2–3 posts you've written as `.txt` or `.md` files in the same folder. These are public, so there's no privacy concern.
- **Option 3 — Write a reply to a sample email (no personal content needed):** Open `sample-data/tone-reference-emails/sample-incoming-email.md`, read the email, then write your reply in a new file called `my-reply.md` in that same folder. Your reply becomes your tone sample.

**How to add a file to the tone-reference-emails folder:**
1. In the Bob Explorer panel, right-click `sample-data/tone-reference-emails/`
2. Select **New File** and give it a name like `email-1.md`
3. Paste your content in and save (`Cmd+S` / `Ctrl+S`)

**Step 1:** In the Bob chat panel, ask Bob to review your tone reference material:
```
Read the emails in sample-data/tone-reference-emails/ and get a sense of how I typically write: tone, greeting/sign-off style, sentence length, level of formality.
```

**Step 2:** Ask Bob to draft a follow-up email:
```
Then draft a follow-up email to the vendor about the invoice discrepancy from the email chain, using that same voice.
```

**If you skipped the tone reference files, use this instead:**
```
Draft a professional follow-up email to the vendor about the invoice discrepancy from the email chain. Keep it concise and polite.
```

**Step 3:** Give Bob one round of feedback:

**Example Prompt (with tone reference emails provided):**
```
Read the emails in sample-data/tone-reference-emails/ and get a sense of how I typically write:
tone, greeting/sign-off style, sentence length, level of formality.

Then draft a follow-up email to the vendor about the invoice discrepancy from the email chain,
using that same voice.
```

**Example Prompt (no tone reference emails, generic tone):**
```
Draft a professional follow-up email to the vendor about the invoice discrepancy from the email chain.
Keep it concise and polite.
```

```
Good, but I'm more direct than that in real emails; trim the pleasantries and get to the ask faster.
```

**Expected Outcome:**
- Bob produces a draft that's ready to send with light editing, not a generic template
- With tone reference material: the draft sounds recognizably like you, not like a generic AI assistant
- Without tone reference material: Bob still produces a solid professional draft as a fallback

**💡 Real-time Value Indicator:**
Drafting a follow-up email from scratch typically takes 5–10 minutes once you factor in re-reading context and getting the tone right. Bob produces a tone-matched first draft in seconds, leaving you to just review and send.

> 💡 **Under the Hood:** This exercise uses the `tone-matched-drafting` skill — a custom Bob skill that reads your reference material, builds a model of how you write, and applies it when drafting. Bob activated it automatically. See [`resources/bob-differentiators.md`](../resources/bob-differentiators.md) to learn more about how custom skills extend Bob.

> 🧭 **Want to explore?** If you have a few extra minutes:
> - "What if I asked Bob to try a more casual tone?" → `Rewrite the email draft but make it more casual — I'm on good terms with this vendor.`
> - "What if I asked Bob to cut it to 3 sentences?" → `Cut this draft down to 3 sentences. Keep only the ask.`
> - "What if I asked Bob to describe my writing style back to me?" → `Based on the emails I shared, describe how I typically write — tone, formality, sentence style.`

---

---

## 🔄 Try This Before You Move On

You've covered all three exercises. Before heading to the next lab, try this in the Bob chat panel:

```
Show me my complete to-do list including everything from all three exercises.
```

Notice that Bob remembers the tasks you added in Exercise 1, the action items it extracted in Exercise 2, and any updates made in Exercise 3 — all within a single conversation.

---

## 🧭 Keep Exploring

You've covered the core of this lab. Bob can go further — here are some things worth trying if you still have time:

- **Bring something real:** Paste in an actual email you need to respond to right now and ask Bob to draft a reply in your tone.
- **Ask Bob what it would do differently:** `Looking at the to-do list and the action items you extracted, what would you do differently if you were managing my day?`
- **Test Bob's memory:** `Without looking back, summarize everything we've worked on since the start of this conversation.`

> 💡 The sample prompts throughout this lab are a starting point. Feel free to ask Bob anything you're curious about — including how it works. If something surprises you, ask a facilitator. That's what they're here for.

---

## 🎓 Key Takeaways

After completing this lab, you should understand:

1. **Conversational Task Tracking**
   - Bob can maintain a running to-do list without a separate app
   - Add, complete, and reprioritize tasks just by describing changes
   - No formatting or manual upkeep required

2. **Multi-Source Synthesis**
   - Bob can extract action items, owners, and deadlines from unstructured text
   - Multiple sources (meetings, emails) can be merged into one clean list
   - Overlaps and unclear ownership get flagged instead of silently duplicated

3. **Tone-Matched Writing**
   - Bob can learn your writing style from a small sample of your own emails
   - Reference material only needs to demonstrate tone, not identical content
   - Without a reference sample, Bob defaults to a solid generic professional tone

4. **Best Practices**
   - Be specific about what's "yours" vs. someone else's when merging tasks
   - Give feedback in one clear round rather than many small tweaks
   - Treat Bob as a first-draft partner; review before sending anything

## 💡 Tips for Success

1. **Start Real:** Use your own actual tasks in Exercise 1 if comfortable; it makes the value obvious
2. **Be Specific:** "Mark the budget summary done" works better than "update my list"
3. **Trust the Merge:** Let Bob do the deduplication in Exercise 2 rather than pre-sorting yourself
4. **One Round of Feedback:** In Exercise 3, give one clear piece of feedback rather than many small edits
5. **Skip Exercise 3 If Needed:** It's optional; Exercises 1 and 2 stand on their own

## 🐛 Common Issues

### Issue: Bob's to-do list doesn't reflect a recent change
**Solution:** Be explicit: "mark X as done" or "remove X" rather than assuming Bob inferred it

### Issue: Merged action items include things that aren't actually yours
**Solution:** Ask Bob to flag ownership explicitly before merging: "tell me who owns each item first"

### Issue: The tone-matched email doesn't sound like you
**Solution:** Add more reference emails (aim for 3–6) or give Bob more specific feedback about what feels off

### Issue: Not sure which tool to use
**Solution:** Ask Bob! "What's the best way to [accomplish task]?"

## 📝 Discussion Questions

1. How does having Bob maintain your to-do list compare to a notes app or task tracker you use today?
2. What's the risk of merging action items from multiple sources without human review?
3. How much of your own writing style could Bob pick up from just 3–6 emails?
4. Where else in your day could "extract action items from this" save you time?
5. What would you *not* want to hand off to Bob, even if it could technically do it?

## ✅ Completion Checklist

- [ ] Completed Exercise 1: Bob-maintained to-do list
- [ ] Completed Exercise 2: Meeting + email action item extraction and merge
- [ ] Completed Exercise 3 (optional): Tone-matched email draft
- [ ] Comfortable asking Bob to track, update, and reprioritize tasks
- [ ] Comfortable asking Bob to synthesize action items across sources
- [ ] Understand how reference material shapes Bob's writing tone

## 🚀 Next Steps

Once you've completed this lab:

1. **Try it with your own content** — feed Bob your actual inbox or a real meeting transcript and see how the patterns from this lab apply to something you work with every day.

2. **Strengthen your voice match** — add more of your own emails to the tone reference folder. The more examples Bob has, the closer the drafts will sound to you.

3. **Continue to your next lab** — choose based on your role and how you spend most of your time:
   - **Lab 2 — Research** (`Lab 2 - Research/instructions.md`) — ideal for analysts, consultants, and anyone whose day-to-day involves reading documents, synthesizing information, and producing written deliverables
   - **Lab 3 — Developer Efficiency** (`Lab 3 - Developer Efficiency/instructions.md`) — ideal for developers, data engineers, and technical practitioners who work in code daily

4. **Bring a real task list** — in your next Bob session, start with your actual recurring to-do list instead of sample data. The workflow is identical; the value is immediate.


## 📚 Additional Resources

- **Bob Differentiators**: See [`resources/bob-differentiators.md`](../resources/bob-differentiators.md) - Learn what makes Bob unique
- **Bob Documentation**: https://ibm.biz/bob-doc
- **Tool Reference Guide**: See [`resources/cheat-sheet.md`](../resources/cheat-sheet.md)
- **Troubleshooting**: See [`resources/troubleshooting.md`](../resources/troubleshooting.md)

### 🌟 Want to Learn More About Bob's Unique Capabilities?

Check out [`resources/bob-differentiators.md`](../resources/bob-differentiators.md) to learn about:
- **Extensible Architecture** - Custom modes, MCP server integrations, and Marketplace
- **Intelligent Optimization** - Automatic model selection and context management
- **Bob Findings** - Automated security and quality analysis
- **Agentic Workflows (v2)** - Sub-tasks, sub-agents, parallel execution, and pre-built workflows
- **Enterprise Modernization** - Java and legacy code transformation

---

**Need Help?** Ask your facilitator or use the dedicated support channel!

## 💰 Business Impact

This lab demonstrates how Bob accelerates everyday knowledge work, not just coding tasks:

### ⏱️ Productivity Gains
- **Task Tracking**: Eliminates manual to-do list upkeep in a separate app
- **Action Item Extraction**: Turns a 10–15 minute re-read of a transcript or email thread into a few seconds
- **Multi-Source Synthesis**: Merges overlapping action items instead of manually cross-checking two sources
- **Email Drafting**: Produces a tone-matched first draft in seconds instead of 5–10 minutes from scratch

### 🐛 Quality Improvements
- **Consistency**: Nothing gets missed when Bob extracts action items from long or messy transcripts
- **Ownership Clarity**: Ambiguous or unassigned action items are flagged rather than silently dropped
- **Tone Accuracy**: Draft emails sound like the participant instead of generic AI output

### 💵 Cost Savings
- **Reduced Manual Effort**: Based on IBM Client Zero's Documentation and Analysis & Insights categories, synthesis-style tasks like this see 95–100% time-savings gains at scale ([`resources/bob-productivity-gains-client-zero.md`](../resources/bob-productivity-gains-client-zero.md))
- **Faster Follow-Through**: Less time between a meeting/email and an action being tracked or acted on
- **Everyday Applicability**: Unlike dev-focused exercises, this lab's time savings apply to any knowledge worker's daily routine

**Estimated Weekly Value per Participant**: 20–30 minutes saved per meeting/email-heavy day on task tracking and follow-up drafting alone

---
