# React + Vite + Storybook

This is a learning sandbox for exploring [Storybook](https://storybook.js.org/) with React and plain CSS.

## Getting Started

Clone the repo, then from the project folder:

```bash
npm install
```

This installs everything the project needs. Run it once after cloning, and again any time `package.json` changes.

## Available Commands

| Command | What it does |
|---|---|
| `npm run dev` | Starts the actual React app at `http://localhost:5173` |
| `npm run storybook` | Starts Storybook at `http://localhost:6006` — this is where you'll spend most of your time |
| `npm run build` | Builds the app for production (won't be needed for this project) |
| `npm run build-storybook` | Builds a static, shareable version of Storybook (not needed yet, but good to know exists) |

## Project Structure

- `src/components/` — your React components live here
- `src/components/*.stories.jsx` — each component's Storybook file, showing its different states/props
- Each component has a matching `.css` file for styling

## Learning Storybook

Start Storybook with `npm run storybook`, then explore the example components already in the sidebar. When you're ready, try creating a new component + story pair from scratch — that's the core loop of how Storybook works.

---

## About this template

This project uses [Vite](https://vite.dev/) to run React, with either [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) or [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) for fast refresh during development. Neither requires any action from you — this is just background info if you're curious.




## Git Workflow

Anything in `<angle brackets>` is a placeholder. Replace it, brackets included.

### Getting started each session

| Command | What it does |
|---|---|
| `cd Desktop/<project-folder>` | Change Directory: moves Terminal into the project folder (for this repo: `Desktop/my-storybook-app`) |
| `pwd` | Print Working Directory: shows which folder I'm in right now |
| `code .` | Opens the current folder in VS Code (`.` means "this folder") |
| `cd ..` | Goes up one folder |

### Everyday commands

| Command | What it does |
|---|---|
| `git status` | Shows which branch I'm on and what's changed since my last commit |
| `git add .` | Stages all changed files (gets them ready to commit) |
| `git add <path/to/file>` | Stages just one file (e.g. `src/stories/button.css`) |
| `git commit -m "<message>"` | Saves staged changes to my local history. The message should describe what changed and why. Don't forget `-m` |
| `git push` | Sends my commits up to GitHub |
| `git pull origin main` | Brings the latest `main` from GitHub down to my computer |
| `git branch` | Lists my local branches. `*` marks the one I'm on |
| `git checkout <branch-name>` | Switches to a branch that already exists (e.g. `git checkout main`) |
| `git checkout -b <branch-name>` | Creates a new branch and switches to it |
| `git branch -d <branch-name>` | Deletes a local branch (safe delete: only works if it's merged). `-D` forces it |

### The loop: one branch per ticket

0. `cd Desktop/<project-folder>`, to get into the project
1. `git checkout main`, so I start from main (local)
2. `git pull origin main`, so main is up to date (from GitHub)
3. `git checkout -b <branch-name>`, a branch for the work
4. `code .` to open the project in VS Code, then make changes and save
5. `git add .` to stage my changes, then `git commit -m "<what I did>"` to save them to my local history with a message
6. `git push` to send my commits to GitHub (the first push of a new branch needs `git push --set-upstream origin <branch-name>`, and Terminal will show me the exact line)
7. Open a PR on GitHub, review it, merge it
8. Back to step 1, then delete the old branch with `git branch -d <branch-name>`

### Good to know

- **Local vs. remote:** my computer and GitHub are two separate copies. Deleting a branch on GitHub doesn't delete it locally.
- **`git stash` / `git stash pop`:** sets changes aside, then brings back the most recent ones.
- **`git restore <filename>`:** throws away changes to a file I haven't committed. This can't be undone.
- **Stuck in Vim?** Press `Esc`, type `:wq`, press `Enter`.
- **`Ctrl + C`:** stops a running server like `npm run storybook`.
- **`npm run storybook`:** starts Storybook at `http://localhost:6006`
