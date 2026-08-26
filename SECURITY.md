# Security and privacy reporting

Pripev handles voice recordings of people's families, photographs of their homes, and
material about relatives who may have died. A vulnerability here is not only a
technical problem, so this policy covers privacy failures alongside the usual ones.

## Reporting

**Use GitHub's private vulnerability reporting** on the affected repository:
*Security* → *Report a vulnerability*. It is private, it reaches the maintainer, and it
keeps the report out of a public issue while it is being fixed.

Please do not open a public issue for anything in the scope below. If private reporting
is unavailable to you, open a public issue containing **only** the sentence "I would
like to report a security issue privately" and nothing else, and you will be contacted.

A dedicated security address will replace this once the domain is registered.

## In scope

- Access to a capsule, recording, transcript, image or export by anyone the owner did
  not grant it to, including through a guessable or leaked link.
- An access code, invite link or revoked grant that keeps working after revocation.
- Anything that causes an original recording or image to be modified, replaced or
  destroyed, or that breaks its hash chain.
- A private capsule appearing in a public listing, search index, cache or CDN.
- Secrets, API keys, tokens or provider responses committed to a repository or exposed
  by a running service.
- Family material appearing in logs, error reports, analytics or a third-party service
  that was not disclosed as a subprocessor.
- Payment, quote or ledger manipulation.

## Also in scope, and treated the same way

- A capsule that cannot be reconstructed from its own exported archive.
- A deletion request that leaves data behind past its stated retention.
- Content that should never have been generated: an invented measurement, a silently
  corrected transcript, or an unapproved fragment reaching a published page.

These are correctness failures in a product whose entire promise is fidelity, and they
are handled with the same urgency as a data leak.

## What we ask

Give us a reasonable window to fix the problem before disclosing it. Do not access,
download, modify or retain anyone else's family material while investigating – if you
can demonstrate an issue against your own capsule or a test fixture, please do that
instead. Do not run automated scanning against production.

## What you can expect

An acknowledgement within a few days, an honest assessment of whether it is a real
issue, and credit in the fix if you want it. This is a one-person project in
development; there is no bounty programme, and pretending otherwise would be dishonest.
