# hi releases

Signed releases of `hi`, the HIPS command line that starts coding agents with HIPS models and a HIPS sign-in (https://hips.com).

This repository holds what `hi` and its installers download and check:

- the release archives for macOS, Linux and Windows, with a signed `SHA256SUMS`, published with each release;
- the signed list of coding-agent versions tested with `hi` on each system;
- `model-tests/record.json` and its signature: which catalog models were tested with which coding agent, in which pool, on which date.

Every signed file is checked against the public keys built into `hi` itself, never against a key taken from this repository.

No release has been published yet.
