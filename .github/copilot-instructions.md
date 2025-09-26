# Copilot Instructions for P5.js-review

## Project Overview
This project is a minimal P5.js sketch review workspace. It is intended for rapid prototyping and experimentation with P5.js in a browser environment. The codebase currently consists of an `index.html` file and a placeholder `README.md`.

## Architecture & Patterns
- **Single-File Entry Point:** All code is loaded via `index.html`. There are no separate JS or CSS files; scripts and styles should be embedded directly or loaded via CDN.
- **P5.js Integration:** Use the P5.js CDN for all sketch logic. Place your sketch code inside `<script>` tags in `index.html`.
- **No Build Step:** There is no build system, bundler, or transpiler. All changes are reflected immediately in the browser.
- **No Test Framework:** There are no automated tests or test runners. Manual browser testing is the norm.

## Developer Workflow
- **Edit & Preview:**
  - Edit `index.html` directly for all code changes.
  - Open the file in a browser to preview changes. Use Live Server or similar tools for auto-reload if desired.
- **Adding P5.js:**
  - Reference P5.js via CDN in a `<script src="https://cdn.jsdelivr.net/npm/p5@latest/lib/p5.min.js"></script>` tag.
  - Place sketch logic in a `<script>` block after the P5.js import.
- **Debugging:**
  - Use browser DevTools for debugging and inspecting canvas output.

## Conventions
- **All-in-One HTML:** Keep all logic in `index.html` unless the project is expanded.
- **Minimal Markdown:** The `README.md` is a placeholder and does not contain workflow or architectural details.
- **No External State:** There is no backend, database, or persistent state.

## Example: Adding a P5.js Sketch
```html
<!-- index.html -->
<script src="https://cdn.jsdelivr.net/npm/p5@latest/lib/p5.min.js"></script>
<script>
function setup() {
  createCanvas(400, 400);
}
function draw() {
  background(220);
  ellipse(200, 200, 50, 50);
}
</script>
```

## Key Files
- `index.html`: Main entry point for all code and sketches.
- `README.md`: Project placeholder; update if project scope expands.

## External Dependencies
- [P5.js CDN](https://cdn.jsdelivr.net/npm/p5@latest/lib/p5.min.js)

---

**If the project expands, update this file to document new workflows, build steps, or architectural changes.**
