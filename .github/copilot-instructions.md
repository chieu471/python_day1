## Purpose

This repository is a minimal learning/tutorial Python project (single-file examples). These instructions give an AI coding agent concise, actionable context so it can be productive immediately.

## Big picture

- Layout: examples live under `Learn_Python/python_day1/`. Current example: `hello.py` — a single-line script that prints a greeting.
- Architecture: there is no service/packaging boundary: code is procedure-style Python scripts rather than a packaged library or application. Treat each file in `python_day1/` as an independent example or exercise.

## What to expect / constraints

- No build system, no tests, no virtualenv config, and no external dependencies in the repository as-is.
- Target runtime: CPython 3.x on Windows (PowerShell is the dev shell in use). Keep changes small and self-contained.

## Developer workflows (concrete)

- Run an example (PowerShell):

```powershell
python .\hello.py
```

- Linting / tests: none present. If adding linting or tests, follow lightweight, single-file approaches (e.g., add a small pytest test next to the example) and include instructions in `README.md`.

## Project-specific patterns and conventions

- Examples are minimal and intended for learning; prefer explicit, easy-to-read code (no advanced packaging, no implicit imports).
- Filenames are short and descriptive: `hello.py` demonstrates a top-level script with side-effect (prints to stdout).
- Avoid adding large dependency manifests. If a dependency is required, add a `requirements.txt` at repo root and document its usage.

## Integration points and external dependencies

- Currently none. If integrating with external services, document credentials and mocks in new files under a `docs/` or `tests/` folder; do not hard-code secrets.

## Examples to reference

- `python_day1/hello.py` — single-line example; AI edits should preserve the intention of small, self-contained examples.

## Guidance for code changes

- Keep PRs minimal and focused (single example or small refactor).
- When editing an example, include a one-line comment at the top describing the intent (e.g., `# Simple script that prints a greeting`).
- If you introduce new files or dependencies, update `copilot-instructions.md` and add usage steps to the repository root README.

## When to ask the user

- If a proposed change introduces packaging, test frameworks, or CI, ask before proceeding — the repo is intentionally minimal.

---
If anything here is unclear or you want the file expanded with additional workflows (testing, CI, packaging), tell me which areas to expand and I will update this file.
