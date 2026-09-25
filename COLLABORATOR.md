# Collaborator guide — Maynooth DZ demo

Instructions for designers and other collaborators working on this site.

**Repo:** https://github.com/Matrix-Internet/maynooth-demo  
**What you’ll edit:** files inside the `website/` folder  
**Live site:** https://maynooth-dz-demo.netlify.app

---

## 1. One-time setup

1. Install **Git** if needed: https://git-scm.com/downloads
2. Install **Cursor** (recommended IDE): https://cursor.com — see [Using Cursor](#using-cursor-recommended) below
3. Accept the GitHub invite (check your email, or open the repo link above)
4. Open **Terminal** (Mac) or **Git Bash** (Windows) and run:

```bash
cd ~/Downloads
git clone https://github.com/Matrix-Internet/maynooth-demo.git
cd maynooth-demo
```

5. Open the project in Cursor: **File → Open Folder…** and choose the `maynooth-demo` folder (not only `website/`)
6. Preview the site locally (Terminal in Cursor: `` Ctrl+` `` / `` Cmd+` ``):

```bash
cd website
python3 -m http.server 8080
```

Open http://localhost:8080 in a browser. Stop the server with `Ctrl+C`.

---

## Using Cursor (recommended)

[Cursor](https://cursor.com) is the recommended editor for this project. It works like VS Code, with a file tree, search, Git tools, and an AI chat that can help with HTML/CSS edits.

### Open the project

1. Clone the repo (step 4 above), or if you already have it: **File → Open Folder…**
2. Select the **`maynooth-demo`** folder (the one that contains `website/`, `README.md`, and this file)
3. In the left sidebar, expand **`website/`** — that’s where all pages, styles, scripts, and `assets/` live

### Tips for this site

- **Start in `website/`** — edit `index.html`, `styles.css`, page-specific `.css` / `.js` files, and images under `website/assets/`
- **Don’t move or rename files** unless the team agrees — links and image paths depend on current names
- **Preview in the browser** — run the local server (above), then refresh after each save to see changes
- **Find text fast** — `Cmd+Shift+F` (Mac) / `Ctrl+Shift+F` (Windows) to search the whole project (e.g. a headline you want to change)
- **Open a file by name** — `Cmd+P` / `Ctrl+P`, type `index.html` or `take-action`
- **Git in the sidebar** — click the branch icon (Source Control) to see changed files, write a commit message, and push (same as the commands below)
- **AI chat (optional)** — open Chat (`Cmd+L` / `Ctrl+L`), describe the change (e.g. “Tighten the hero spacing on mobile in styles.css”), and review the suggested edits before accepting. Prefer small, clear requests; always check the preview after accepting
- **Ask about a selection** — highlight HTML/CSS, then ask Chat what it does or how to adjust it
- **Stay on `main`** unless someone asks you to use a branch — pull before you start, push when you’re done

### Keyboard shortcuts worth knowing

| Action | Mac | Windows |
|--------|-----|---------|
| Open file by name | `Cmd+P` | `Ctrl+P` |
| Search in project | `Cmd+Shift+F` | `Ctrl+Shift+F` |
| Save | `Cmd+S` | `Ctrl+S` |
| Toggle terminal | `` Cmd+` `` | `` Ctrl+` `` |
| AI chat | `Cmd+L` | `Ctrl+L` |
| Source Control (Git) | `Ctrl+Shift+G` | `Ctrl+Shift+G` |

VS Code also works if you prefer it, but Cursor is what the team recommends for editing and committing this demo.

---

## 2. Before you start work each day

```bash
cd ~/Downloads/maynooth-demo
git pull
```

That downloads the latest changes so you don’t overwrite someone else’s work.

---

## 3. Make your changes

- Edit HTML, CSS, JS, and images in **`website/`** only
- Keep filenames the same unless you’ve agreed a rename
- Preview again with the local server above

---

## 4. Commit and push your work

```bash
cd ~/Downloads/maynooth-demo
git status
git add .
git commit -m "Short description of what you changed"
git push
```

Examples of good commit messages:

- `Update hero copy on homepage`
- `Replace retrofit project image`
- `Fix spacing on take-action page`

---

## 5. If `git push` asks you to sign in

Use your GitHub username, or a **Personal Access Token** if GitHub asks for a password:

GitHub → Settings → Developer settings → Personal access tokens

Alternatively, use **GitHub Desktop**: https://desktop.github.com — clone the same repo, edit files, then **Commit** and **Push**.

---

## Quick cheatsheet

| Goal | Command |
|------|---------|
| Get latest | `git pull` |
| See what changed | `git status` |
| Save + upload | `git add .` → `git commit -m "..."` → `git push` |

---

## Deploy note

Pushing to GitHub does **not** automatically update the live Netlify site yet. After you push, tell the team so it can be redeployed.
