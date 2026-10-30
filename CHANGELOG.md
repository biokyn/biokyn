# Changelog

## 1.1.0
Fixed many security issues found in first version.

## 1.0.0
First stable release. RFC 9497 ristretto255-SHA512 VOPRF verified against the official vectors, token v2, Argon2id proof-of-work, WebAuthn lane, Redis-backed stores, Express and Next.js adapters.

## 0.4.0-rc.1
Added: RFC 9497 VOPRF; token v2 with key ids and key ring; anonymous WebAuthn registration + credential stores + counter checks; trusted-proxy IP resolution, IPv6 bucketing, route-aware rate limiter;
fail-closed Redis guard (timeouts, 503), cluster hash tags; Redis integration, fuzz and property tests; evaluation (Wilson CI) and load-test tooling; accessible motion dialog; CI (Redis matrix, vectors gate, CodeQL, Dependabot);
deployment, incident-response, data-retention, privacy, threat-model, accessibility and evaluation documents.
Changed (breaking): wire version 2; motion/kinematics advisory-only; `/motion-step-up` response; `@noble/*` 2.x; `LIVENESS_SCRIPT` wrapper; `dist/` no longer shipped.
Fixed: `HashToScalar` byte order; contradictory/flaky tests; type errors under TS ≥ 5.9; duplicated adapter route list.
