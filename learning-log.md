# Learning Log · Full-Stack MVP in 5 Weeks

Nov 3 – Dec 7, 2026 · Goal: finish the frontend, learn backend basics, ship a production-ready MVP.

**How to use:** every evening, copy the template, paste it under "Entries" (newest day on top), and fill it in. Each morning, paste yesterday's entry into Claude and type `PLAN`.

## Day __ · YYYY-MM-DD · Week __

**Goal:**
**Status:** ✅ Done / 🟡 Partly / ❌ Not done. **Why:**

### 🛠️ Built
-

### 📚 Learned
-

### 💻 Code
| Snippet | What it does |
|---------|--------------|
| `` | |

### ❓ Still Fuzzy
- [ ]

### 🧱 Problems → Fixes
- →

### 📊 Wrap-up
- **Quiz:** _/5 · weak spot:
- **Commit:**
- **Hours:**
- **Tomorrow first:**
- **Reflection:**

Repo: https://github.com/partanihomayoun-blip/learning-log



## Days 2026-11-08 + 2026-11-09 · Week 1

**Goal:** Build a basic Google homepage clone and practise flexbox
**Status:** 🟡 Partly. **Why:** Skipped Nov 8 (no excuse). Did the work on Nov 9.

### 🛠️ Built
- Basic Google clone layout with light styling
- Practised `display: flex` for the overall layout

### 📚 Learned

**Layout: ask this first**
- Should the items in this section **stack** (column) or sit **side by side** (row)?

**Flexbox**
- `display: flex` on the parent puts its children in a row.
- `justify-content` only decides *where* they sit on that row: start, center, end or spread out.
- `gap` only works on a flex or grid container.

**Box sizing**
- `border-box`: the width you set is the whole box. Padding and border go inside, so the content shrinks.
- `content-box`: the width you set is only the content. Padding and border are added outside, so the box gets bigger.
- The content itself never grows, only the total box.

**Inline elements (`<a>`)**
- `<a>` is inline. It ignores top/bottom margin; left/right margin still works.
- Fix: `display: inline-block;` makes vertical margin work.

**Forms**
- `type="search"` is for `<input>`, not `<button>`.
- `type="button"` = the button does nothing by default.
- A `<button>` inside a `<form>` with no type acts as **submit**.

**Save for later:** the "visually hidden" pattern.

### 💻 Code
| Snippet | What it does |
|---------|--------------|
| `* { box-sizing: border-box; }` | Makes every element use border-box sizing |
| `display: flex;` | Lines children up in a row |
| `flex-direction: row / column;` | Side by side or stacked |
| `justify-content: center;` | Positions items along the row |
| `gap: 16px;` | Space between flex/grid children |
| `flex: 1;` | Item grows to fill the leftover space |
| `display: inline-block;` | Inline element that accepts vertical margin |
| `margin` / `padding` | Space outside / inside the border |
| `border: 1px solid black;` | Draws a border |
| `border-radius: 24px;` | Rounds the corners |
| `color` / `background-color` | Text colour / background colour |
| `font-family` / `font-size` | Typeface / text size |

### ❓ Still Fuzzy
- [ ] Inline vs block vs inline-block elements
- [ ] Cascading and descendant selectors (e.g. `nav a`)
- [ ] When and where to use `<div>`

### 🧱 Problems → Fixes
- Margin on `<a>` did nothing vertically → `display: inline-block`

### 📊 Wrap-up
- **Quiz:** _/5 · weak spot:
- **Commit:**
- **Hours:** 3h
- **Tomorrow first:**
- **Reflection:**

Repo: https://github.com/partanihomayoun-blip/learning-log

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
