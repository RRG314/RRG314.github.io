# Validation and Testing

Validation is an important part of this work, particularly for the computational projects.

## PRNG Testing

The RGE-256 generators were tested using established statistical test suites, including Dieharder.

Summary:
- No core generators fail Dieharder
- At least one core was independently tested and validated
- External testing led to reengineering and improved variants
- Testing influenced revisions to both code and papers

The PRNG work is used as an experimental probe of recursive entropy theory rather than as a cryptographic claim.

## Iterative Revision

One PRNG paper was endorsed for submission to arXiv but did not pass moderation. Since then, revisions have incorporated feedback on clarity, framing, and presentation. The version history reflects that process.

This site is intended to document that progression openly rather than present a single static result.
