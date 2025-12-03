<!--
Sync Impact Report:
- Version change: 1.0.0 → 2.0.0
- List of modified principles:
    - "Spec-Driven Development (SDD)" → "I. Project Scope"
    - "Clean Code & Project Structure" → "II. Architecture Rules"
    - "Comprehensive Functionality" → "III. Coding Standards"
    - "Clear Documentation & Repository Structure" → "IV. CLI Rules"
    - "Technology Stack" → "V. Spec-Kit Compatibility"
    - Added: "VI. Output Rules"
- Added sections: None
- Removed sections: "Technology Stack", "Development Workflow & Deliverables"
- Templates requiring updates:
    - .specify/templates/plan-template.md ⚠ pending
    - .specify/templates/spec-template.md ⚠ pending
    - .specify/templates/tasks-template.md ⚠ pending
    - Command files in .specify/templates/commands/*.md ⚠ pending
    - README.md ⚠ pending
    - GEMINI.md ⚠ pending
- Follow-up TODOs: None
-->
# Phase 1: In-Memory Python Todo CLI Application Constitution

## Core Principles

### I. Project Scope
This phase is strictly limited to an in-memory Python Todo CLI application. No database, web server, API, or external frameworks are permitted. The focus is on pure, clean Python logic.

### II. Architecture Rules
A simple Python project structure must be used: `/models` for the Task model, `/services` for the TaskService (add, view, update, delete, complete), and `main.py` for the CLI loop only. All business logic must reside within the services, not in `main.py`. No external dependencies beyond the Python standard library are allowed.

### III. Coding Standards
Python 3.13+ type hints must be used everywhere. Code must be readable, clean, and beginner-friendly, with English comments for clarity. Unnecessary complexity is forbidden, and functions must be small and single-purpose.

### IV. CLI Rules
The CLI must support the following commands: `add <task-title>`, `update <id> <new-title>`, `delete <id>`, `complete <id>`, `view`, and `exit`. The CLI must provide clear error messages for invalid input. No external CLI libraries are to be used; only `input()` and `print()` are permitted.

### V. Spec-Kit Compatibility
The AI must always follow the specifications located in the `/specs/` folder. In case of any conflict, the specification takes precedence over this constitution. All generated code must map 1-to-1 with the Phase 1 specifications.

### VI. Output Rules
Code generation is strictly confined to the boundaries of Phase 1. Future-phase features such as databases, APIs, or UIs are not to be introduced. All outputs must remain minimal, predictable, and spec-driven.

## Governance

The AI agent must always ask for permission before adding new files and must adhere to the 'single responsibility per file' principle. The agent must never assume future architecture and must stick strictly to Phase 1 guidelines. This Constitution is the single source of truth for Phase 1 development.

**Version**: 2.0.0 | **Ratified**: 2025-12-03 | **Last Amended**: 2025-12-03