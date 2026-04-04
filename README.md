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

Pushing to `master` triggers the GitHub Actions workflow in `.github/workflows/deploy.yaml`.

That workflow installs dependencies, runs the Sass build, and deploys the contents of `dist/` to the `gh-pages` branch.

## Quick Update Flow

```bash
npm install
npm run sass
# edit files
npm start
# commit changes
# push to master
```
