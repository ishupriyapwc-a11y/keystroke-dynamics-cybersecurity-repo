```markdown
# Contributing

Thanks for your interest in contributing to this project. This document explains how to propose changes, submit experiments, and contribute data safely and ethically.

Ground rules
- This repo is for defensive, research, and educational purposes only. Do NOT add code that captures keystrokes from devices you do not own or manage.
- All contributions must respect privacy and informed consent. Any code, data, or instructions that interact with real users require clear consent and secure handling.

How to contribute
1. Open an issue first for non-trivial features or datasets so we can discuss scope and safety.
2. Fork the repository and create a branch for your change:
   git checkout -b your-feature-name
3. Make changes, add tests, and update documentation/notebooks as needed.
4. Commit with clear messages and submit a Pull Request to main. Describe safety/privacy considerations in the PR body.

Tests and CI
- Add tests under `tests/` for new functionality.
- The CI runs pytest and a synthetic example. Ensure new code passes the existing test suite.

Real-data contributions (required checklist)
If you intend to contribute experiments using real typing data, you MUST include:
- The signed consent form template filled by participants (see `CONSENT_FORM.md`).
- A written description of the data collection environment (OS, keyboard type, task text, sampling method).
- A data anonymization plan (how identifiers are removed) and a secure storage plan (encryption, access controls).
- A summary of the intended use and retention period for the data.
Contributions that don’t include this documentation will be rejected.

Data handling and security best practices
- Store raw data encrypted at rest and limit access to authorized researchers only.
- Keep personally identifying information (PII) separate from measurement data and use an irreversible identifier mapping if needed.
- Share only anonymized or synthetic datasets in the repo; do not upload raw consenting data to the public repository.

Code style & documentation
- Follow PEP8 for Python code.
- Add a short notebook or README for experiments that reproduces the key steps and random seeds used.
- Document model evaluation procedures and metrics.

License and attribution
- Contributions will be accepted under this repository’s license (see LICENSE).
- If your contribution includes third-party data/code, include attribution and license information.

Contact & support
- Open an issue or tag @maintainers in PRs if you need help. For sensitive topics (data privacy, consent forms), discuss in an issue before uploading anything.
```
