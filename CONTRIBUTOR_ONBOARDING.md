Onboarding Guide for Contributors to the ROSS‑OS Constitutional Substrate
Welcome to the ROSS‑OS Constitutional Substrate.
This guide will help you understand the architecture, workflow, and expectations for contributing to the deterministic kernel that underpins Ross‑OS, CopWan Ledger Physics, Trinity Prism, Everlight 24, and all Ross‑native systems.

This onboarding guide is intentionally concise and practical — it gets you productive quickly while preserving the substrate’s invariants.

1. Understand the Purpose of the Substrate
Before contributing, ensure you understand what this repository is and is not.

The substrate is:

the deterministic governance kernel

the constitutional root‑of‑trust

the canonicalization + hashing + lineage engine

the foundation for all Ross‑OS runtimes

The substrate is not:

an application layer

a UI

a domain‑specific runtime

a place for nondeterministic logic

For a conceptual overview, start with:
Constitutional Substrate Overview

2. Learn the Core Invariants
Every contribution must preserve:

determinism

replay‑safety

canonicalization consistency

lineage integrity

cluster symmetry

immutable genesis and root‑of‑trust

If unsure whether a change affects invariants, open a discussion via:
Start determinism review

3. Explore the Repository Structure
The repo is organised into:

/docs/ — architecture, invariants, module specs

/src/ — deterministic modules

/tests/ — unit tests for each subsystem

/tools/ — validators, analyzers, simulators

Start by reading:
Constitutional Stack Map  
Runtime Flow

4. Set Up Your Environment
You’ll need:

Python 3.10+

deterministic‑safe libraries only

no randomness, no time‑dependent behaviour, no external state

Install dependencies and run tests:

Code
pip install -r requirements.txt
pytest
5. Making Your First Contribution
Step 1 — Open an Issue
Describe the change you want to make:
Open substrate issue

Step 2 — Create a Branch
Use the naming convention:

Code
feature/<module>-<short-description>
fix/<module>-<short-description>
Step 3 — Implement the Change
Follow module headers and deterministic rules.

Step 4 — Add Tests
Every change requires a corresponding test in /tests/.

Step 5 — Submit a PR
Submit via:
Submit substrate pull request

6. When to Request a Constitutional Review
You must request a constitutional amendment review if your change affects:

genesis

canonicalization rules

hashing model

lineage semantics

freeze/recovery logic

Request via:
Request amendment review

7. Getting Help
If you’re unsure where to start, ask:
Where should I begin contributing?

If you need architectural guidance:
Explain substrate architecture

8. Welcome Aboard
Thank you for contributing to the deterministic foundation of the Ross‑OS ecosystem.
Your precision strengthens every system built on top of this substrate.
