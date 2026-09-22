# Team Project — Resolving Conflict in GitHub

## 🔗 Repository Link (Public)
https://github.com/arminedjlal-eng/team-project

> This repository is **Public** and available for review.

---

## 📌 Project Summary

This project is a hands-on exercise for resolving conflicts in GitHub using **Merge** and **Rebase**. Two simultaneous changes were made to the `team_project.txt` file, and the resulting conflict was resolved in two different ways.

---

## 🌿 Branch Structure

| Branch | Description | Final commit |
|---|---|---|
| `main` | Main branch | `cefdf7c` |
| `feature-a` | Conflict resolution with **Merge** | `66d8cc6` |
| `feature-rebase` | Conflict resolution with **Rebase** | `aad381d` |

---

## 📝 Project Steps

### Step 1: Create branch and push to Remote
- Create branch `feature-a`
- Add `Feature A implemented` to `team_project.txt`
- commit: `e101bf6` — `feat: add Feature A to team_project.txt`
- push to GitHub

### Step 2: Simulate simultaneous change
- Edit `team_project.txt` on `main`
- Add `Feature B implemented`
- commit: `f28f200` — `feat: add Feature B to team_project.txt`

### Step 3: Pull and create Conflict
- On `feature-a`: `git pull origin main`
- conflict in `team_project.txt`

### Step 4: Resolve Conflict with Merge
- Manual edit: keep both features
- commit: `66d8cc6` — `merge: resolve conflict between Feature A and Feature B`
- push to GitHub

### Step 5: Review changes with Rebase
- Create branch `feature-rebase` from `main`
- Add `Feature C implemented (rebase practice)`
- Parallel change on `main`: `Feature D implemented (main change)` — commit: `cefdf7c`
- `git rebase main` → conflict
- Resolve conflict + `git rebase --continue`
- **Linear and clean history** — commit: `aad381d`
- push to GitHub

### Step 6: Teamwork best practices
- Compare Merge and Rebase
- Clear commit messages
- Coordinate branches before push

---

## 📊 Merge vs Rebase Comparison

| Feature | Merge | Rebase |
|---|---|---|
| History | Has merge commit | Linear and clean |
| commit hash | Two-parent | One-parent |
| Use case | Public branches | Personal branches |
| Risk | None | Rewriting history |

---

