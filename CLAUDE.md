# CLAUDE.md

Instructions for AI coding agents working in this repository.

## How we work together

I'm building this project to learn and to show what I can do. I own the design and the core code.

- **Explain before you change.** For anything beyond a trivial fix, propose a plan and wait for my approval.
- **Don't write core logic for me.** Connectors, dbt models and analysis code are mine to write. Point me in the right direction, review what I wrote, and ask questions that challenge my choices.
- **Boilerplate is fine.** You may draft config files (CI workflows, `pyproject.toml`, pre-commit), but explain every line you add.
- **Tell me why.** When you suggest an approach, name at least one alternative and the trade-off.

<!-- TODO: Adjust these rules once you've tried them for a week. Which ones help, which get in the way? -->

## Data and privacy

- Never read, print or copy anything under `data/` or any `.env` file. Use the synthetic data in `synthetic/` instead.
- Never add real health data to code, tests, fixtures, commit messages or issues.

## Project conventions

- Language: English for code, comments, commit messages and docs.
- Python tooling: `uv` for dependencies, `ruff` for linting and formatting.
- Commit messages: <!-- TODO: pick a convention, e.g. Conventional Commits (feat:, fix:, docs:) -->
- Every pull request closes an issue (`Closes #N`) and passes CI before merge.

## Commands

<!-- TODO: Fill in as the project grows. -->

```bash
# make demo     # generate synthetic data, run the pipeline, start the app
# make test     # run pytest and dbt tests
```

## Architecture

See `README.md` for the data flow and `docs/decisions/` for the reasoning behind key choices.