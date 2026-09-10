---
title: Contributor Guide
description: How to add problems and concepts to CTRI Math
---

Welcome! This guide will help you start contributing to CTRI Math — even if you have never used GitHub or Obsidian before. You do not need to be a developer. If you can type and follow steps, you can contribute.

## What you will be doing

You will be writing **Problems** (questions with worked solutions) and **Concepts** (short explanations of mathematical ideas). These get linked together to build a knowledge graph that students can explore.

---

## Part 1 — One-time setup

### Step 1 — Create a GitHub account

GitHub is where all the content is stored. Think of it like Google Drive, but built for files that a team edits together.

1. Go to [github.com](https://github.com) and click **Sign up**
2. Enter your email, create a password, and choose a username
3. Verify your email address
4. Send your GitHub username to the Team Lead so you can be added to the project

### Step 2 — Accept your invitation

1. Check your email for an invitation from GitHub
2. Click **Accept invitation**
3. You now have access to the CTRI Math content

### Step 3 — Install GitHub Desktop

GitHub Desktop is a simple app that lets you download the content, make changes, and submit them — no technical commands needed.

1. Go to [desktop.github.com](https://desktop.github.com) and download it
2. Install and open it
3. Sign in with your GitHub account

### Step 4 — Clone the repository

"Cloning" means downloading a copy of the content to your computer.

1. In GitHub Desktop, click **File → Clone repository**
2. Click the **URL** tab
3. Paste: `https://github.com/careforknowledge/ctri-math-content`
4. Choose where to save it on your computer
5. Click **Clone**

You now have a copy of all the content on your computer.

### Step 5 — Install Obsidian

Obsidian is the app you will use to write and edit content. It works like a notebook where pages can link to each other.

1. Go to [obsidian.md](https://obsidian.md) and download it
2. Install and open it
3. Click **Open folder as vault**
4. Find the `ctri-math-content` folder you just cloned and open it

You should see folders on the left: **Concepts**, **Exams**, **Problems**, **Topics**.

### Step 6 — Install the LaTeX Suite plugin

When you open the vault in Obsidian for the first time, it will ask if you trust the vault. Click Trust vault. All plugins are already installed and ready.

**Useful shortcuts after installing:**
- Type `mk` → becomes `$...$` (for inline math like $x^2$)
- Type `dm` → becomes `$$...$$` (for display math on its own line)
- Type `//` inside math → becomes `\frac{}{}`

---

## Part 2 — Every time you contribute

### Step 1 — Create a branch

A branch is your own personal workspace. You make all your changes there, and only when a reviewer approves does it go into the main site. This keeps mistakes off the live site.

1. Open GitHub Desktop
2. Make sure you are in the `ctri-math-content` repository
3. Click **Current branch** at the top
4. Click **New branch**
5. Name it something descriptive, for example: `amina-waec-2015-algebra`
6. Click **Create branch**

You are now working in your own branch.

### Step 2 — Write your content in Obsidian

Open Obsidian. You should see your branch name reflected in your working copy. Now add your content using the templates below.

#### Adding a Problem

Create a new file inside the **Problems** folder. Name it like this:

```
waec-2015-q3.md
neco-2019-q11.md
original-quadratic-001.md
```

Use this template:

```
---
title: "Write a short version of the question here"
type: problem
source: "[[Exams/waec-2015|WAEC 2015]]"
difficulty: medium
concepts:
  - "[[Concepts/completing-the-square|Completing the Square]]"
---

## Question

Write the full question here. For inline math use $x^2 + 3x = 0$ and for display math use:

$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

## Solution

Write the full worked solution here. Show every step. Do not skip steps — a student who has never seen this before should be able to follow.
```

**Difficulty guide:**
- `easy` — straightforward application of one concept
- `medium` — requires combining two ideas or a few steps
- `hard` — multi-step, requires insight or multiple concepts

#### Adding a Concept

Create a new file inside the **Concepts** folder. Name it in lowercase with hyphens:

```
quadratic-formula.md
number-bases.md
simple-interest.md
```

Use this template:

```
---
title: Concept Name Here
type: concept
topic: "[[Topics/algebra|Algebra]]"
---

Write a clear, simple explanation of this concept. Imagine you are explaining it to an SS2 student who is seeing it for the first time.

## Key Formula

$$\text{put the main formula here if there is one}$$

## Related Concepts

- [[Concepts/related-concept|Related Concept Name]]

## Problems

- [[Problems/waec-2015-q3|WAEC 2015 Q3]]
```

### Step 3 — Check your work in Obsidian

Before submitting, switch to **Reading view** in Obsidian (click the book icon top right) and check:
- Does all the LaTeX render correctly?
- Are the links clickable and pointing to real files?
- Is the solution clear and complete?

### Step 4 — Submit your work

When you are happy with your content:

1. Open **GitHub Desktop**
2. You will see your changed files listed on the left
3. At the bottom left, write a short summary of what you added — for example: *Add WAEC 2015 Q3 — completing the square*
4. Click **Commit to [your branch name]**
5. Click **Push origin** at the top

### Step 5 — Open a Pull Request

1. In GitHub Desktop, click **Create Pull Request** (it will appear after you push)
2. This opens GitHub in your browser
3. Write a short title and a brief description of what you added
4. Click **Create pull request**

That is it! A reviewer will check your work. You will get an email notification when it is approved and live, or if there are changes requested.

---

## Tips for good contributions

- Always show every step in a solution
- Write in simple English — the reader is an SS2 student
- Link every problem to at least one concept
- If the concept you need does not exist yet, create it
- Check your LaTeX in Reading view before submitting
- One branch per contribution keeps things clean

## Need help?

Reach out to the Team Lead or email hello@ctri.ng.

---

*Prefer the terminal? See the [[Contributors/terminal-path|Terminal Path]] for command-line instructions.*
