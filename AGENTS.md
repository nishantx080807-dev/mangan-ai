# Mangan-AI Development Instructions

## Current Phase

The repository is currently in the AUDIT phase.

Do NOT modify application code unless explicitly instructed.

## Core Rules

1. Understand existing code before changing it.
2. Do not delete existing files.
3. Do not rewrite working modules unnecessarily.
4. Do not introduce dependencies without justification.
5. Do not change API contracts without documenting the change.
6. Do not hardcode secrets, credentials, API keys, or passwords.
7. Never commit `.env` files or credentials.
8. Preserve existing functionality unless a replacement is explicitly approved.
9. Prefer small, testable changes.
10. Run appropriate tests after implementation changes.
11. Do not force-push Git branches.
12. Do not modify unrelated files.

## Architecture Principles

Keep these concerns logically separated:

- frontend
- backend/API
- database/storage
- data ingestion
- preprocessing
- machine learning
- inference
- visualization

The backend should not contain frontend-specific logic.

The ML layer should expose predictable interfaces so the API does not depend on implementation-specific model details.

## AI Development Rule

Before implementing a major feature:

1. Inspect the existing implementation.
2. Identify dependencies.
3. Explain the proposed change.
4. Identify affected files.
5. Implement the smallest coherent change.
6. Test it.
7. Explain what changed.

## Current Objective

First understand the existing Mangan-AI repository completely.

Do not redesign the architecture until the current architecture has been documented.
