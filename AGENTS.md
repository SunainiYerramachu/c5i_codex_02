# Repository Guidelines

## Project Structure & Module Organization

This repository is a self-contained training lab for comparing Codex behavior with and without project instructions.

- `learner/starter/src/checkout.py` implements `calculate_total(items)`.
- `learner/starter/tests/test_checkout.py` contains the checkout unit tests.
- `learner/starter/sample_orders.json` provides synthetic example data.
- `learner/starter/task_card.md` defines the discount and formatting exercises.
- The starter README and comparison worksheet describe the experiment and evidence to record.
- `learner/skill_and_mcp_lab.md` and `learner/integration_task_template.md` support integration exercises.

Keep checkout implementation and tests in their existing directories. Preserve an untouched baseline copy when conducting the comparison; create a separate guided copy as described in the starter README.

## Build, Test, and Development Commands

Run checks from the checkout project directory:

```sh
cd learner/starter
python3 -m unittest discover -s tests -v
```

On Windows, use `python` or `py` if `python3` is unavailable. In a guided copy, run the same command from that copy's root. No package installation, compilation, development server, formatter, or linter is configured.

## Coding Style & Naming Conventions

Follow the existing Python style: four-space indentation, `snake_case` functions and variables, double-quoted strings, and short docstrings for public functions. Use `CamelCase` for test classes and `test_` prefixes for test methods.

Preserve the item schema (`name`, `price`, `quantity`) and the float return contract of `calculate_total`. Keep display formatting separate from calculation. Do not introduce dependencies for the supplied exercises.

## Testing Guidelines

Use standard-library `unittest`. Add focused cases to `tests/test_checkout.py` for changed behavior, boundary values, and expected errors. Preserve existing empty-cart and float-return tests. Follow the task card's required cases when implementing an exercise. No coverage threshold is configured; run the complete suite before submitting changes.

## Commit & Pull Request Guidelines

Commit history could not be inspected because Git was unavailable in the authoring environment. Use concise, imperative commit subjects, such as `Add discount boundary tests`.

Pull requests should describe the behavior changed, identify the exercise or issue, list verification commands and results, and explain any public-contract changes. For lab submissions, include the comparison worksheet and the requested reflection. Use synthetic data; never commit credentials or real customer/payment information.
