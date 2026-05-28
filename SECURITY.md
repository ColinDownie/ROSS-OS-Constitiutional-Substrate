Security Policy for the ROSS‑OS Constitutional Substrate
The ROSS‑OS Constitutional Substrate is the deterministic governance kernel that underpins Ross‑OS, CopWan Ledger Physics, Trinity Prism, Everlight 24, and all Ross‑native systems.
Because this repository defines the constitutional root‑of‑trust, security is a first‑order concern.

This document outlines how to report vulnerabilities, how they are handled, and the expectations for responsible disclosure.

1. Supported Versions
Only the following versions of the substrate receive security updates:

v1.x.x — Active support

v0.x.x — Best‑effort support (pre‑1.0 experimental series)

Versions below v0.5.0 are considered archival and do not receive security patches.

For versioning details, see:
Substrate Versioning Model

2. Reporting a Vulnerability
If you discover a security issue, please report it privately and responsibly.

Use one of the following channels:

Submit a private security report

Request a security review

Please include:

a clear description of the issue

steps to reproduce

affected modules (canonicalization, hashing, lineage, etc.)

potential impact

suggested mitigations (if known)

Do not open a public GitHub issue for security vulnerabilities.

3. What Constitutes a Security Issue
Security issues include:

nondeterministic behaviour in canonicalization or hashing

lineage corruption or replay divergence

bypassing freeze, recovery, or governance rules

dependency graph manipulation

activation‑tick manipulation

any behaviour that breaks cluster symmetry

any behaviour that compromises the root‑of‑trust

If unsure, submit via
Ask if this is a security issue.

4. Response Process
Once a report is received:

A maintainer acknowledges receipt within 72 hours

The issue is reproduced and classified

A fix is developed in a private branch

A patch release is prepared

The reporter is notified before public disclosure

The fix is merged and documented

Critical issues may trigger a constitutional freeze, handled according to:
Freeze & Recovery Protocol

5. Responsible Disclosure
We ask that reporters:

do not publicly disclose vulnerabilities before a fix is released

avoid exploiting or weaponising the issue

coordinate disclosure timelines with maintainers

This ensures the substrate remains stable, deterministic, and safe for all downstream systems.

6. Thank You
Security researchers and contributors play a vital role in maintaining the integrity of the ROSS‑OS ecosystem.
Your diligence helps protect every system built on this constitutional foundation.
