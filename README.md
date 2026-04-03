# sridharnandigam.github.io

Small static personal site with Sass source files in `scss/` and compiled output in `dist/`.

## Requirements

- Node.js and npm

## Install

```bash
npm install
```

## Run Locally

Start the Sass watcher in one terminal:

```bash
npm run sass
```

Serve the built site from `dist/` in another terminal:

```bash
npm start
```

Then open:

```text
http://localhost:8000
```

## Project Structure

- `scss/`: source Sass files
- `dist/`: compiled site that gets deployed
- `dist/css/main.css`: generated from `scss/`
- `dist/js/main.js`: client-side JavaScript

## Deployment

This repo already includes a deploy script:

```bash
npm run deploy
```

That command publishes `dist/` using the `gh-pages` package.

Deployment notes:

- You need push access to `origin` and working GitHub auth on this machine.
- The current remote is `git@github.com:sridharnandigam/sridharnandigam.github.io.git`.
- The current working branch is `master`.
- `npm run deploy` assumes GitHub Pages is configured to serve the `gh-pages` branch.
- Since this is a static site, make sure any edits in `scss/` have been compiled into `dist/` before deploying.

## Quick Update Flow

```bash
npm install
npm run sass
# edit files
npm start
# when ready
npm run deploy
```
