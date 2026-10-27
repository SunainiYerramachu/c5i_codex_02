---
name: checkout-change
description: Implement or revise Tiny Shop Checkout behavior, its unittest coverage, and related API documentation. Use for checkout feature changes in this lab, not unrelated Python work or MCP setup.
---

# Checkout Change

Use the current task's acceptance criteria to guide the change. Work in the selected guided checkout project; preserve the starter baseline.

## Inspect the contract

Read applicable `AGENTS.md` instructions, `src/checkout.py`, `tests/test_checkout.py`, and the relevant task in `task_card.md`. Read the project README for local verification instructions.

Before editing, briefly identify the existing public contract, the requested behavior, and files likely to change. The current checkout accepts items with `name`, `price`, and `quantity` and returns a float, including `0.0` for an empty cart. Preserve existing calls unless the user requests a contract change. Keep currency formatting in a separate helper. If a request changes that contract, explain the effect on callers and tests.

## Implement and verify

- Implement only the requested behavior; do not implement other task cards automatically or introduce dependencies for the supplied exercises.
- Add focused standard-library `unittest` cases for the acceptance criteria, relevant boundaries, and expected errors. Retain existing contract tests unless the requested contract changes.
- Update the project README when public behavior changes, showing the relevant call and result.
- From the selected checkout project's root, run `python3 -m unittest discover -s tests -v`. Use `python` or `py` on Windows when appropriate. If no Python interpreter is installed, report that verification is blocked; do not claim tests passed.
- Inspect the diff for unrelated changes, changed input/output contracts, and accidental baseline edits. If Git is unavailable, inspect changed files directly and disclose the limitation.

## Report

Summarize the behavior implemented, files changed, and actual verification command and result. State any remaining uncertainty or untested behavior. Skill creation alone does not authorize implementing an exercise or connecting external services.
