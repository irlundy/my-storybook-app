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


## Additional 