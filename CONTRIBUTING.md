# Contributing

Thank you for looking. Please read the two hard rules before anything else.

## Two hard rules

**No family material, ever.** No recording, transcript, photograph, cutout or export
derived from a real family goes into any repository in this organisation, public or
private. Fixtures are synthetic or separately and explicitly consented. Repository
storage is not publication consent, and a private repository is not a safe place for
someone else's voice.

**No secrets, ever.** No API key, token, `.env` file, or raw provider response.
Credentials reach a process through the environment. Usage receipts are redacted before
they are written down.

Both of these are checked in review, and a pull request that trips either one is closed
rather than amended.

## How the organisation is laid out

Most of this work is private while it is being built. The repository that is open is
**`cookbook-agent`**, the bounded editorial agent that composes a capsule page from an
approved transcript and an approved set of visual fragments. **`capsule`**, the document
schema and portable archive format, opens before launch, because a promise that a family
can rebuild their capsule without us is only worth something if the format is public.

If you want to contribute code, those are the places.

## The boundary that matters most

The agent decides meaning. Deterministic code decides geometry.

The agent chooses what the recording says, how it should be structured, which fragments
belong where, and what the page should feel like. It never calculates a coordinate,
writes CSS, invents a font family, or edits an approved transcript. The layout engine
places, wraps, collides and paginates, and never makes an editorial decision.

Changes that blur this line will be asked to move to one side of it.

## Things the product will not do

Proposals for these are declined on principle rather than on merit, so please do not
spend time on them:

- Generating, cloning or synthesising anyone's voice.
- Supplying external cooking guidance, or filling in a measurement, temperature or time
  that was not said out loud.
- Inferring age, health, cognition or ethnicity from speech.
- Correcting a transcript silently, or altering an approved one.
- Applying a cultural theme derived from a language, surname or country.
- Generic system fonts in a finished page.

## Working style

- Small pull requests that do one thing.
- Explain **why** in the description; the diff already shows what.
- Match the surrounding code. There is no house style document, and there does not need
  to be one.
- Prose in Markdown uses en dashes, not em dashes.
- If a change touches how a capsule is stored or rendered, say what happens to capsules
  that already exist.

## Tests

A change to editorial behaviour needs a fixture that fails before it and passes after.
This is the only way to tell an improvement apart from a different opinion, and it
applies to skill files as much as to code.

## Reporting problems

Security and privacy issues go through [SECURITY.md](SECURITY.md), privately, not
through a public issue.
