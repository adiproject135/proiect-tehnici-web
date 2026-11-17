# UNSOLVED

UNSOLVED is a responsive digital-forensics investigation website built for the Tehnici Web course.

## The case

A confidential file was accessed from HOST-04 outside normal working hours. The site presents the workstation logs and four fictional rooms. Each room contains a different security clue:

- **Alex:** login details left on a note attached to the monitor.
- **Maria:** a password note hidden under the keyboard.
- **David:** a password based on his name, written on the blackboard.
- **Victor:** personal interests and routines that could support a targeted phishing attempt.

All names, accounts, log entries and credentials are fictional.

## Current implementation

Phase 1 uses semantic HTML5 and CSS3. The location menu uses the native `details` and `summary` elements. Room interactions are made with checkbox inputs and CSS selectors. There is no JavaScript or backend in this version.

The layout adapts to desktop, tablet and mobile screens. Keyboard focus styles and reduced-motion preferences are also supported.

## Run locally

Open `index.html` in a browser, or start a local server from this directory:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Project files

- `index.html` — title screen and entry point.
- `pages/investigation.html` — HOST-04 workstation, login history and room directory.
- `pages/alex.html`, `pages/maria.html`, `pages/david.html`, `pages/victor.html` — the four room scenes and their clues.
- `css/variables.css` — shared colors, fonts and layout values.
- `css/main.css` — base styles and shared utilities.
- `css/layout.css` — page layout and responsive rules.
- `css/components.css` — navigation, panels, badges and terminal styles.
- `css/pages/` — styles for the intro, investigation and room pages.
- `assets/` — images and illustrations used in the scenes.
- `materials/req.md` — course project requirements.

The site is a static prototype. The terminal and investigation records are visual examples; they do not run commands or access a real system.
