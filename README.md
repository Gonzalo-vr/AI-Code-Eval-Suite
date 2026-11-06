# AI-Code-Eval-Suite

A reproducible evaluation framework designed to test the software engineering capabilities of frontier AI models. This suite contains isolated environments with deterministic verifiers to evaluate LLMs on performance optimization, async debugging, and code refactoring.

## Architecture

Each directory in this repository represents a standalone Reinforcement Learning (RL) environment tailored for AI agent evaluation:
- **Problem Statement:** Defines the task, constraints, and success criteria.
- **Buggy/Legacy Code:** The starting point for the AI model.
- **Verifier:** Deterministic tests (often with strict execution time limits) that accept valid implementations and reject incorrect or hard-coded solutions.
- **Golden Solution:** A reference implementation demonstrating an optimal approach.

## Environments

1. `01-python-performance-opt`: Tests the model's ability to identify $O(n^2)$ complexity bottlenecks and optimize them to $O(n)$ using appropriate data structures.
2. `02-js-async-bug-fix`: Evaluates the model's handling of JavaScript event loop mechanics, race conditions, and concurrent Promise execution.
