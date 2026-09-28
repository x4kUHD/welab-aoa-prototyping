# Agent instructions

This repo is for **HTML prototyping** only. It exists to quickly visualize and demo feature ideas — not to build production code.

## Rules

- Write **pure HTML, CSS, and vanilla JS**. No frameworks, no build step, no bundlers (React, Vue, Next.js, Tailwind CLI, webpack, vite, etc. are all off-limits).
- No `npm install` of UI/framework dependencies. The only tooling in this repo is a static file server (`npm run dev`).
- Every prototype is a single self-contained folder under `prototypes/<name>/` with its own `index.html`. Prefer one `index.html` per prototype with inline `<style>`/`<script>`, unless sharing code across prototypes clearly helps — in which case put it in `shared/`.
- To start a new prototype, copy `prototypes/example/` and edit it. Add a link to it from the root `index.html`.
- It's fine (and encouraged) to use plain `<script>` tags to pull in a CDN library (e.g. Chart.js, Alpine.js) directly in HTML if it helps a prototype, as long as it doesn't require a build step.
- Keep prototypes disposable and readable over "correct" — this is for exploring and reviewing ideas, not shipping.
- Don't add TypeScript, JSX, CSS preprocessors (Sass/Less), or package managers beyond what's already in `package.json`.
