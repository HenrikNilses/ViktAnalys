# Copilot instructions

## Project context
- This repository is a simple static web application / single-page application (SPA).
- Keep the app client-side and deployable as static files. Do not introduce a backend, database, build system, or runtime dependency unless the task explicitly requires it.
- Follow the technologies and conventions already present in the repository. If the project is still empty or has no established stack, prefer simple HTML, CSS, and vanilla JavaScript.

## Implementation guidelines
- Make focused, minimal changes that solve the requested task; avoid unrelated refactors and unnecessary dependencies.
- Keep code readable and split it into small, reusable pieces when that improves clarity. Use descriptive names and add comments only where the intent is not obvious.
- Use semantic HTML and accessible controls. Ensure keyboard navigation, visible focus states, useful labels, and sufficient color contrast.
- Make layouts responsive and usable on both narrow mobile screens and larger screens.
- Validate and handle user input safely. Do not use `innerHTML` with untrusted or user-provided content; prefer safe DOM APIs such as `textContent`.
- Keep application state and persistence straightforward. Use browser storage only when appropriate, and handle missing or invalid stored data gracefully.
- Do not add analytics, external services, or collect personal data unless explicitly requested.

## Security and secrets
- Never store, commit, log, expose, or hard-code private keys, passwords, access tokens, API keys, or other credentials in source code, configuration, documentation, tests, or repository history.
- Do not ask users to paste secrets into the repository or a prompt. Use environment variables or an appropriate secret manager for credentials when they are required; ensure secret files are excluded from version control.
- If a secret is discovered in the repository, do not repeat it or copy it elsewhere. Flag the exposure and recommend revoking/rotating the credential and removing it from tracked files and history as appropriate.

## Verification
- Before changing files, inspect the existing project structure and follow its established patterns.
- Run the checks and tests that the repository already provides. If no test or build setup exists, verify changes with the available browser or static checks and state what could not be run.
- Update documentation when a change affects how the app is used or developed.
