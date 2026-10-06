# Playwright Daily Lab — Codex Instructions

This repository is a learning project for Playwright with TypeScript.

## Main goal

Help maintain and improve practical Playwright examples without overcomplicating the code.

## Rules

- Use TypeScript.
- Prefer clear and beginner-friendly code.
- Follow Playwright best practices.
- Prefer resilient locators such as `getByRole`, `getByLabel`, `getByTestId`.
- Avoid unnecessary `waitForTimeout()`.
- Keep tests isolated.
- Do not introduce abstractions unless they are actually useful.
- Do not refactor working learning examples without a clear reason.
- Explain important changes briefly.
- Preserve the educational purpose of each test.
- Prefer small focused examples over large complex scenarios.
- Do not modify unrelated files unless necessary.

## Project structure

- `tests/` — practical Playwright examples
- `docs/ROADMAP.md` — learning roadmap
- `docs/LEARNING_LOG.md` — completed sessions
- `docs/CHEATSHEET.md` — quick syntax reference
- `docs/PLAYWRIGHT_NOTES.md` — detailed explanations

## When adding a new learning example

- Put it in the appropriate topic folder under `tests/`
- Keep the test focused on one Playwright concept
- Use a descriptive test name
- Make sure the test passes
- Update documentation only when relevant
