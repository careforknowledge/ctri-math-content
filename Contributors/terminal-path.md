---
title: Terminal Path
description: Command-line instructions for technical contributors
---

This page is for contributors who prefer working in the terminal instead of GitHub Desktop. The process is the same — only the tools differ.

## Clone the repository

```bash
git clone https://github.com/careforknowledge/ctri-math-content.git
cd ctri-math-content
```

## Create a branch

```bash
git checkout -b your-name/description
# example: git checkout -b amina/waec-2015-algebra
```

## After writing your content in Obsidian

```bash
git add .
git commit -m "Add WAEC 2015 Q3 — completing the square"
git push origin your-branch-name
```

Then open a Pull Request on GitHub as described in the [[Contributors/contributor-guide|Contributor Guide]].
