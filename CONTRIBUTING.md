# Contributing to Untrace

Welcome, #untrace.biulders.

Untrace is building privacy infrastructure for the AI breach era: client-side encrypted files, threshold-protected shards, wallet-gated retrieval, audit receipts, and selective disclosure proofs. We like contributions that make the system easier to inspect, easier to run, harder to break, or clearer to explain.

## Ways To Contribute

You do not need to arrive with a giant PR. Useful work comes in many sizes:

- Documentation that makes the architecture easier to understand.
- Reproducible demos, scripts, and local setup improvements.
- Tests, fixtures, and vectors for cryptographic flows.
- Rust node runtime improvements around storage, transport, identity, and receipts.
- Wallet and policy experiments for signed retrieval grants and revocation flows.
- ZK benchmarks, Noir circuits, verifier notes, and proof-size analysis.
- Security review notes, threat model gaps, or abuse-case writeups.
- Frontend prototypes for private vaults, eSignatures, proofs, and escrow workflows.

## Before You Start

1. Read the project README for the protocol shape and current assumptions.
2. Search existing issues and discussions so we can avoid duplicate threads.
3. For bigger work, open an issue first with the problem, proposed direction, and expected tradeoffs.
4. Keep early PRs small. A focused improvement is easier to review and merge.

## Good First Contributions

Great first shards include:

- Clarifying a confusing paragraph or diagram.
- Adding a missing setup step.
- Creating a minimal example for encryption, shard generation, retrieval, or reconstruction.
- Writing tests for nonce, expiry, vault ID, policy context, and signature validation behavior.
- Documenting failure cases: missing shards, expired requests, revoked access, corrupted manifests.
- Benchmarking a proof flow and publishing the exact command, hardware, timing, and output size.

## Contribution Flow

1. Fork or branch from the latest main branch.
2. Make the smallest complete change that solves the issue.
3. Add or update tests/docs when behavior changes.
4. Run the relevant formatter, linter, and tests for the repo you touched.
5. Open a PR with a clear title and a short explanation of what changed.

A good PR description answers:

- What problem does this solve?
- What changed?
- How was it tested?
- What remains out of scope?

## Security And Privacy Rules

Untrace makes strong security claims, so contributions should be careful and boring in the best way.

- Do not commit secrets, keys, real documents, private wallet data, customer data, or production credentials.
- Keep raw document data off-chain.
- Treat access grants as explicit, scoped, signed, and expiring.
- Prefer documented primitives and reproducible benchmarks over clever undocumented shortcuts.
- Call out assumptions in PRs when a design depends on trust, timing, availability, custody, or policy state.
- If you find a serious vulnerability, do not open a public exploit issue. Contact the maintainers privately first.

## Review Style

We review for correctness, clarity, and threat-model fit. Expect questions about edge cases, failure modes, and whether a contribution keeps the data lifecycle private by architecture.

Healthy disagreement is welcome. Personal attacks, harassment, spam, and low-effort token speculation are not.

## Community Energy

Bring build logs, demos, critiques, weird integrations, and useful questions. We are especially excited by contributors who can help others run the local vault demo, explain the architecture, or turn security review into better public docs.

Make the breach meaningless.
