# Repository Guidelines

## Project Structure & Module Organization

This project is Hessa’s interactive birthday storybook. `index.html` contains the page markup, inline CSS, JavaScript, and embedded image assets. `START_HERE.txt` provides browser launch instructions. There are no separate source, test, or build directories.

Personalized content is configured through `window.HESSA_BOOK`, including the name, birthday, gallery captions, wishes, and final letter photo. Its comments describe using relative paths under `assets/photos/` for replacement photos; that directory is not currently included.

## Build, Test, and Development Commands

- Open `index.html` directly in Chrome, Edge, or Safari for the supported local workflow.
- Optionally run `python3 -m http.server 8000 --bind 127.0.0.1` from this directory, then visit `http://127.0.0.1:8000` for HTTP-based preview.
- Use F11 on Windows to check the fullscreen presentation described in `START_HERE.txt`.

No dependency installation, compilation, package scripts, or automated test command is configured. Google Fonts are imported remotely, so check font fallback behavior without connectivity.

## Coding Style & Naming Conventions

Preserve the existing single-file structure and surrounding formatting. Use two-space indentation for expanded HTML and JavaScript blocks, descriptive camelCase JavaScript names, and hyphenated CSS classes such as `.gallery-modal`. Keep existing compact CSS formatting when making focused changes.

Reuse CSS custom properties and existing interaction handlers. Avoid reformatting unrelated sections or modifying long embedded data URLs accidentally. No formatter or linter is configured. Preserve semantic buttons, accessible labels, visible keyboard focus, and reduced-motion styles.

## Testing Guidelines

Validation is manual; no testing framework or coverage threshold exists. After changes, check the entrance door, forward/back navigation, page indicators, sound controls, portrait slider, gallery lightbox, wishes, and final letter. Confirm the Mema photo and signature appear only after the final letter opens.

Check desktop and narrow mobile layouts, keyboard interaction, reduced motion, and browser console errors. Record browsers and interactions checked in the pull request.

## Commit & Pull Request Guidelines

Git history is unavailable in this checkout, so no established message convention can be verified. Use short imperative subjects, for example `Fix gallery layout on narrow screens`.

Keep changes focused. Describe the user-visible result, link an issue when applicable, and include before/after screenshots for visual changes plus manual verification results.
