# Collaborator guide — Maynooth DZ demo

Instructions for designers and other collaborators working on this site.

**Repo:** https://github.com/Matrix-Internet/maynooth-demo  
**What you’ll edit:** files inside the `website/` folder  
**Live site:** https://maynooth-dz-demo.netlify.app

---

## 1. One-time setup

1. Install **Git** if needed: https://git-scm.com/downloads
2. Install a code editor (optional but useful): [Cursor](https://cursor.com) or [VS Code](https://code.visualstudio.com)
3. Accept the GitHub invite (check your email, or open the repo link above)
4. Open **Terminal** (Mac) or **Git Bash** (Windows) and run:

```bash
cd ~/Downloads
git clone https://github.com/Matrix-Internet/maynooth-demo.git
cd maynooth-demo
```

5. Preview the site locally:

```bash
cd website
python3 -m http.server 8080
```

Open http://localhost:8080 in a browser. Stop the server with `Ctrl+C`.

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
