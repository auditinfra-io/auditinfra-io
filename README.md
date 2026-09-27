Static analysis for zero-knowledge circuits and smart contracts.

## Open-source tools

- **[o1js-scan](https://github.com/auditinfra-io/o1js-scan)** — finds witnesses
  the prover controls but the circuit never binds, in o1js / Mina zkApps and
  Noir circuits. A single-file lexical pass with no dependencies, on PyPI and
  npm. Listed in the o1js
  [Community Packages](https://github.com/o1-labs/o1js#community-packages)
  directory.
- **[gnark-safety](https://github.com/auditinfra-io/gnark-safety)** — reports
  gnark hint outputs whose constraints look incomplete, and ten other patterns
  that often mean a circuit accepts values it should reject. Experimental,
  pre-1.0.
- **[vk-guard](https://github.com/auditinfra-io/vk-guard)** — snapshots o1js
  verification-key hashes and per-method constraint counts into a committed
  file, and fails CI when they drift. On npm.

Each tool's README says where it stops. A clean result from any of them is not
an audit, and a finding is a lead to review.

## Audit Engine CLI

A multi-language static analysis and bounded model checking engine for smart
contracts and ZK circuits. The engine is private; its architecture is
documented in public in [audit-engine](https://github.com/auditinfra-io/audit-engine).
