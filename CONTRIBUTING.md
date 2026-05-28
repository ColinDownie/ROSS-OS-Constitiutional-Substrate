Guidelines for contributing to the ROSS‑OS Constitutional Substrate
Thank you for your interest in contributing to the ROSS‑OS Constitutional Substrate.
This repository defines the deterministic governance kernel that underpins Ross‑OS, CopWan Ledger Physics, Trinity Prism, Everlight 24, and all Ross‑native systems. Because this substrate forms the constitutional bedrock, contributions must follow strict rules to preserve determinism, replay‑safety, and cross‑cluster symmetry.

1. Core Principles
All contributions MUST uphold the following invariants:

Determinism — same inputs produce identical outputs across all architectures

Replay‑Safety — historical reconstruction must match live state

Canonicalization Consistency — all data must serialize identically

Lineage Integrity — no mutation of committed lineage

Cluster Symmetry — behaviour must be identical across nodes

Immutable Genesis & Root‑of‑Trust — these cannot be altered

If you are unsure whether a change affects determinism, open a discussion via
Start a determinism review.

2. How to Contribute
Bug Reports
Use clear, reproducible steps. Include:

expected behaviour

actual behaviour

minimal failing example

environment details

Open an issue via
Report a substrate issue.

Feature Requests
Only propose features that:

strengthen determinism

improve clarity

enhance safety

extend documentation

Submit via
Propose a substrate feature.

Pull Requests
PRs must:

modify only the relevant module

include tests in /tests/

update documentation in /docs/

pass determinism checks

avoid introducing nondeterministic libraries or behaviour

Open a PR via
Submit a substrate pull request.

3. Repository Structure
Before contributing, review:

Constitutional Stack Map

Runtime Flow

Canonicalization Engine

Understanding the layering model is essential.

4. Code Style
All code must:

be pure, side‑effect‑free where possible

avoid global state

avoid nondeterministic APIs

follow the deterministic module headers already in /src/

5. Governance of the Substrate
Changes to:

genesis

root‑of‑trust

canonicalization rules

hashing model

lineage semantics

…require a constitutional amendment review via
Request amendment review.

These changes are rare and heavily scrutinized.

6. Thank You
Your contributions help strengthen the deterministic foundation that the entire Ross‑OS ecosystem stands on.
Precision matters here — and your attention to it is appreciated.
