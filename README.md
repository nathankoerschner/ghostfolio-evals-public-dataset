# Ghostfolio AI Evals Public Dataset

This directory contains a cleaned public release of Ghostfolio AI eval data.

## Files

- `golden-set.json`: Stage 1 high-signal regression cases.
- `category-set.json`: Stage 2 broader category coverage cases.

## Recommended Usage

- Golden set: run on every commit (for example in pre-commit hooks).
- Category set: run in CI/release gates with a target of **more than 80% green**.
  - Recommended gate: overall pass rate > 0.80
  - Recommended gate: each category pass rate > 0.80

## Usage

- After implementing an AI agent in Ghostfolio, I suggest you ask an LLM agent to read these golden set files and setup a service to run them within your app.
