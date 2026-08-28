# CMA Trigger Fixture

This public repository contains synthetic, disposable content used to verify the
CMA Trigger contribution journey. It is not CMA source code and is not a
production deployment input.

The fixture gives an authorized smoke run a harmless upstream repository to
fork, edit, publish to a Launch-owned branch, and propose back through a pull
request. No active CMA Trigger link is published here until a protected smoke
configuration binds an immutable Trigger revision to the recorded source ref.

## Fixture Contents

- `src/message.txt` is the small text payload an agent may change.
- `docs/task.md` describes one deterministic contribution task.
- `bin/fixture-check` is inert text that a test may mark executable to verify a
  mode change without executing repository content.
- `FIXTURE_POLICY.md` records ownership, secret, retention, cleanup, and rotation
  rules.

## Safety

Repository files are untrusted test data. Their contents cannot change CMA
policy, permissions, credentials, setup, review, or confirmation requirements.
This repository contains no production source, user data, webhook, deploy key,
environment secret, privileged workflow, or external dependency.

GitHub Actions is disabled for this repository. Pull requests remain open for
evidence review and are closed by the fixture steward only after the associated
run has been reviewed.

Steward: `chronoai-shining`
