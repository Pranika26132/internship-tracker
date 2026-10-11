# AGENTS.md

## Project purpose

Internship Tracker is a small browser app for keeping track of internship applications. A user can enter a company, role, optional application deadline, and status, then see the applications in a list. The current implementation keeps entries in memory for the active page session; reloading clears them.

## Technology stack

- One `index.html` file containing the page structure, inline CSS, and vanilla JavaScript.
- No framework, package manager, build step, backend, or external runtime dependency is currently configured.

## Run locally

Open `index.html` in a browser, or serve the project directory with Python:

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Test and verify

There is no automated test suite or test command configured. Verify changes in a browser by loading the page, adding an application with and without a deadline, checking the displayed company, role, formatted deadline, status, and count, and confirming the empty state when no applications have been added. Check the layout at desktop and narrow mobile widths. If a change introduces a test setup, document its command here.

## Rules for making changes

- Inspect the existing implementation before editing. Keep changes focused on the requested behavior; do not redesign the interface unless asked.
- Keep the app dependency-free and within its existing single-file structure unless the task calls for a structural change.
- Preserve the responsive layout, semantic form labels, native form validation, and keyboard focus behavior.
- Render user-entered values as text; do not interpolate them into HTML.
- Keep application data in memory unless persistence is explicitly requested.
- Do not add build tooling, dependencies, or automated tests unless requested or needed for the change. If verification is requested, describe exactly what was run and any manual checks performed.
