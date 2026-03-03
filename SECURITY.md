# Security Policy

Thank you for helping keep the **nextjs-app-router-snippets** project and its users safe.

> **About this repository**
> This repository provides code snippets and examples for Next.js App Router. It is **not** a production service. However, issues in snippets can still lead to insecure patterns in downstream applications. We treat reports seriously and appreciate responsible disclosure.

## Supported Versions

This project follows a **community-maintained** model:

- We accept security reports for the **default branch** (`main`) and the **latest release**.
- Older tags/archives are **out of scope** unless a critical issue also affects the latest code.

## How to Report a Vulnerability

Please use **GitHub Security Advisory**
> Open a private report via **Security → Report a vulnerability** in this repository.

When reporting, please include:

- A clear description of the issue and potential impact.
- Minimal proof-of-concept or snippet demonstrating the problem.
- Affected file(s) / snippet(s) and commit SHA if possible.
- Suggested remediation (if you have one).

We aim to acknowledge reports **within 7 days** and provide a status update **within 14 days**. Timelines are **best effort** for a volunteer-run project.

## Coordinated Disclosure

We kindly ask researchers to:

- Allow us a reasonable time to **triage**, **fix**, and **publish** before public disclosure.  
- Avoid data destruction, privacy violations, or service disruption during testing.

Once a fix/mitigation is available (or after a mutually agreed window), we will:

- Publish a changelog note and/or release.
- Credit reporters (if desired) in release notes or the advisory.

## Scope

**In scope**

- Insecure code patterns within this repository’s snippets (e.g., auth/session misuse, XSS-prone patterns, SSRF-prone examples, insecure default configurations).
- Documentation that encourages unsafe defaults or misleading guidance.

## Handling Fixes

Because this is a snippets repository:

- Fixes typically land as **documentation updates** or **improved code examples**.
- We strive to keep examples aligned with **current Next.js guidance** and safe defaults.
- We may **deprecate** or **remove** problematic snippets and document safer alternatives.

We encourage users to always:

- Review snippets before use.
- Keep dependencies updated.
- Apply secure coding practices appropriate for their application context.

## Security Hygiene

- No secrets should be committed to this repository. If you find any accidentally committed secret, please report it privately using the channels above.
- We recommend consumers enable **dependency update tooling** and static checks in their own projects.

## Safe Harbor

We support **good-faith** security research:

- If you follow this policy and avoid harming users/data, we will not pursue legal action.
- Do not access, modify, or exfiltrate data without explicit permission.  
- Stop testing and report immediately if you encounter user data or sensitive information.

---

## Contact

- Security reports: **GitHub Security Advisory**

Thank you for helping us improve security for everyone who uses these snippets.
``
