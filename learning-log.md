# Learning Log · Full-Stack MVP in 5 Weeks

Nov 3 – Dec 7, 2026 · Goal: finish the frontend, learn backend basics, ship a production-ready MVP.

**How to use:** every evening, copy the template, paste it under "Entries" (newest day on top), and fill it in. Each morning, paste yesterday's entry into Claude and type `PLAN`.

## Day __ · YYYY-MM-DD · Week __

### 🎯 Goal
- [ ] Main goal:
- [ ] Stretch goal (optional):
- **Status:** ✅ Done / 🟡 Partly done / ❌ Not done. **Why:**

### 🛠️ Built / Practised
- 

### 📚 Learned (in my own words)
#### Concepts
- 

#### Commands / Code
| Command / Snippet | What it does |
|-------------------|--------------|
| `` | |

### ❓ Still Fuzzy
- [ ] 

### ✔️ Resolved (from earlier fuzzy lists)
- 

### 🧱 Blockers / Errors I Hit
- **Problem:** → **Fix:**

### 📝 Quiz
**Score:** _/5

**Weak spots:**
1. 

### 🔗 Commits / Live Link
- Repo: https://github.com/partanihomayoun-blip/learning-log
- Today's commit(s):

### ⏭️ Tomorrow's First Task
- 

### ⏱️ Focused Hours
- 

### 💭 Reflection (1–2 lines)
- What went well / what to change tomorrow:---

## Entries

## Day 2–3 · 2026-11-04 → 2026-11-05 · Week 1

### 🎯 Goal
- Box model + Flexbox + Google clone — **not completed**

### 🛠️ Built / Practised
- Cloned my GitHub repository into a local folder on my PC
- Connected the local repo to GitHub and checked the connection

### 📚 Learned (in my own words)

#### Git workflow — the golden rule
- **Always start in the local folder on my PC**, then push to the GitHub repo.
- If I make a change **on GitHub directly**, I run `git pull` first to bring those changes into my local folder, **then** `git push`. Doing it in this order avoids merge problems.

#### Git commands
| Step | Command | What it does |
|------|---------|--------------|
| 1. Get the repo | `git clone <full-repo-URL-ending-in-.git>` | Copies the whole repository to my PC |
| 2. Check state | `git status` | Shows which files are changed / staged (only *shows*, changes nothing) |
| 3. Stage | `git add <file-name>` | Puts the changed file in the staging area |
| 4. Commit | `git commit -m "short message explaining the change"` | Saves a snapshot with a message |
| 5. Upload | `git push <remote> <branch>` → e.g. `git push origin main` | Sends my commits to GitHub |
| Sync down | `git pull` | Brings changes from GitHub into my local folder |
| History | `git log --oneline --graph -5` | Shows the last 5 commits in a compact graph |
| Differences | `git diff` | Shows what changed in files *(still fuzzy)* |

#### Fixing a stuck lock file
- `ls .git/index.lock` — check whether the lock file exists
- `rm .git/index.lock` — delete it (use the exact path shown by `ls`)

#### Networking side note
- **MTU (Maximum Transmission Unit):** the biggest packet of data that can travel through a link in one piece.

### ❓ Still Fuzzy
- `git fetch`
- In `git merge origin/main`, what does `origin/main` refer to?
- `git diff`

### 📝 Quiz
**Score:** 3/5

**Weak spots:**
1. The three file states (modified, staged, committed) vs. commands that only *show* state (`git status`)
2. Remote (`origin`) vs. branch (`main`)
3. What a lock file is, and `rm` vs. `git rm`
4. Quotes around commit messages

### 🔗 Commits / Live Link
- https://github.com/partanihomayoun-blip/learning-log

### ⏭️ Tomorrow's First Task
- Box model + Flexbox + Google clone

### ⏱️ Focused Hours
- 1 hour


## Day 1 · 2026-11-03 · Week 1

### 🎯 Goal
- Set up the Claude Project and this learning-log repo — **completed**

### 🛠️ Built / Practised
- Created the Claude Project (instructions + playbook PDF)
- Created the `learning-log` repo on GitHub
- Created a new file, `learning-log.md`, on the `main` branch and committed it on GitHub

### 📚 Learned (in my own words)
- How to create a new repository on GitHub
- How to create a new file inside that repository and commit it directly on GitHub

### ❓ Still Fuzzy
- How to clone a repo to my local PC and commit from there

### 📝 Quiz
**Score:** 5/5

**Weak spots:**
- None for now

### 🔗 Commits / Live Link
- https://github.com/partanihomayoun-blip/learning-log

### ⏭️ Tomorrow's First Task
- Box model + Flexbox; finish the Google clone

### ⏱️ Focused Hours
- 30 minutes
