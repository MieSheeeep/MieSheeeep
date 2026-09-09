# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a `MieSheeeep` profile README using the approved brunotacca-inspired structure.

**Architecture:** Keep the profile in one standalone Markdown file. Use HTML comments as edit markers, shields.io for technology badges, and username-parameterized external cards for live GitHub statistics.

**Tech Stack:** GitHub Flavored Markdown, inline HTML, shields.io, GitHub README Stats, Streak Stats, Komarev counter

---

### Task 1: Replace the profile README

**Files:**
- Modify: `README.md`

- [x] **Step 1: Record the current validation failure**

Run: `rg -n "About Me|Main Tech Stack|github-readme-stats.*MieSheeeep" README.md`

Expected: no matches because the file contains only the repository title.

- [x] **Step 2: Write the complete profile**

Replace `README.md` with the approved sections: introduction, editable personal bullets, contact link, primary skills, learning skills, GitHub statistics, and visitor count. Put `<!-- 修改区 N -->` before every user-editable group and use `MieSheeeep` in every dynamic GitHub URL.

- [x] **Step 3: Validate attribution cleanup and dynamic usernames**

Run: `rg -n "brunotacca|brunotacca@gmail.com|cint.com|ko-fi.com" README.md`

Expected: no matches.

Run: `rg -n "MieSheeeep" README.md`

Expected: matches in the title and every GitHub statistics/visitor URL.

Run: `rg -n "修改区" README.md`

Expected: edit markers for personal text, contact details, primary skills, and learning skills.

- [x] **Step 4: Check formatting and commit**

Run: `git diff --check`

Expected: no output and exit code 0.

Run: `git add README.md docs/superpowers/plans/2026-09-09-profile-readme.md && git commit -m "feat: build GitHub profile README"`

Expected: one commit containing the README and this implementation plan.
