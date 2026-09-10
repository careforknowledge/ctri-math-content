---
title: Reviewer Guide
description: How to review and approve content submissions for CTRI Math
---

Thank you for being a reviewer. Your role is important — you are the quality check that makes sure everything on CTRI Math is mathematically correct, clearly written, and properly formatted before it goes live.

This guide will walk you through the review process step by step.

---

## What reviewers do

When a contributor finishes adding content, they submit it for review by opening a **Pull Request (PR)**. You will get an email notification. Your job is to:

1. Read through the content
2. Check it is correct and clearly written
3. Either approve it (it goes live) or ask for changes

You do not need to be a developer to do this. The process is straightforward.

---

## Step 1 — Find the Pull Request

1. Go to [github.com/careforknowledge/ctri-math-content/pulls](https://github.com/careforknowledge/ctri-math-content/pulls)
2. You will see a list of open Pull Requests
3. Click on one to open it
4. Click the **Files changed** tab to see what the contributor added or changed

---

## Step 2 — Preview the content in Obsidian

The best way to review is to see the content rendered exactly as a student would — with equations, links, and formatting all visible. Here is how:

1. Open **GitHub Desktop** and make sure you are in the `ctri-math-content` repository
2. Click **Current branch** at the top and select the contributor's branch (it will be named something like `amina-waec-2015-algebra`)
3. Open **Obsidian** — it will automatically show the content from that branch
4. Switch to **Reading view** (book icon, top right) to see rendered LaTeX and clickable links
5. Browse to the file the contributor added and review it fully rendered

This is the most reliable way to catch LaTeX errors, broken links, and formatting issues before they go live.

> If you cannot switch branches in GitHub Desktop, open a terminal in the `ctri-math-content` folder and run:
> `git fetch origin` then `git checkout branch-name`

---

## Step 3 — What to check

Work through this checklist for every Pull Request:

**The mathematics**
- [ ] Is the question stated clearly and completely?
- [ ] Is the solution correct?
- [ ] Are all steps shown? A student who has never seen this topic should be able to follow.
- [ ] Is the difficulty level (`easy`, `medium`, `hard`) appropriate?

**The writing**
- [ ] Is the language simple enough for an SS2 student?
- [ ] Is the explanation in the concept note clear?

**The formatting**
- [ ] Does the filename follow the naming convention? (`waec-2015-q3.md`, `completing-the-square.md`)
- [ ] Is the frontmatter complete? Check for `title`, `type`, `source`, `difficulty`, and `concepts`
- [ ] Does the LaTeX render correctly in Obsidian's Reading view?

**The links**
- [ ] Is the problem linked to at least one concept?
- [ ] If a new concept was created, is it linked to a topic?
- [ ] Does the concept file link back to the problem?

---

## Step 4 — Leave feedback

If something needs fixing, do not just reject it — explain clearly what is wrong and what should change. Contributors are learning.

1. Click the **Files changed** tab
2. Hover over the line you want to comment on — a blue **+** icon will appear on the left
3. Click it and write your comment
4. When you have finished all your comments, click **Finish your review**
5. Select **Request changes** and click **Submit review**

The contributor will get an email and can make the changes, then re-request your review.

---

## Step 5 — Approve and merge

When everything looks good:

1. Click **Review changes** (top right of the Files changed tab)
2. Select **Approve**
3. Click **Submit review**
4. Click **Merge pull request**
5. Click **Confirm merge**

The site will automatically rebuild. New content will be live at `math.ctri.ng` within a few minutes.

---

## Common issues and how to handle them

**LaTeX not rendering correctly**
Ask the contributor to open the file in Obsidian's Reading view, fix the equation, and resubmit.

**Broken links**
A link like `[[Concepts/completing-the-square]]` will break if that file does not exist. Either ask the contributor to create the missing file, or create a simple stub yourself.

**Incorrect solution**
Leave a comment explaining the error as clearly as possible. If you are not certain yourself, escalate to the Team Lead — do not merge content you are unsure about.

**Solution is correct but unclear**
Ask the contributor to rewrite the explanation more simply. A good test: would an SS2 student who has never seen this topic understand it step by step?

**Naming convention not followed**
Ask the contributor to rename the file. Do not merge with the wrong filename — it will be difficult to fix later.

---

## When to escalate to the Team Lead

Do not merge if:
- You are not confident the mathematics is correct
- The content seems inappropriate for secondary school students
- A contributor is unresponsive to feedback
- You are unsure about anything at all

In any of these cases, leave a comment tagging `@` the Team Lead's GitHub username and explain the situation. They will take it from there.

---

## A note on tone

Contributors have put effort into their submissions. When asking for changes, be kind and specific. A good review comment says *what* is wrong and *how* to fix it — not just that something is wrong.

Thank you for helping maintain the quality of CTRI Math.
