# hi releases

Signed releases of `hi`, the HIPS command line that starts coding agents with HIPS models and a HIPS sign-in (https://hips.com).

## Install

On macOS and Linux:

```sh
curl -fsSL https://hips.com/hi.sh | sh
```

On Windows, in PowerShell:

```powershell
irm https://hips.com/hi.ps1 | iex
```

With Homebrew:

```sh
brew install hips-ai/tap/hi
```

The newest release is at https://github.com/hips-ai/hi-releases/releases/latest, and the documentation at https://hips.com/docs/cli.

## What this repository holds

This repository holds what `hi` and its installers download and check:

- the release archives for macOS, Linux and Windows, with a signed `SHA256SUMS`, published with each release;
- the signed list of coding-agent versions tested with `hi` on each system;
- `model-tests/record.json` and its signature: which catalog models were tested with which coding agent, in which pool, on which date.

Every signed file is checked against the public keys built into `hi` itself, never against a key taken from this repository.

## Report a bug

Open an issue with the bug form: https://github.com/hips-ai/hi-releases/issues/new/choose. It asks for:

- what `hi --version` prints, and your system (for example macOS 15 on Apple silicon, Windows 11 or Ubuntu 24.04);
- the coding agent and the version it prints (for example what `codex --version` prints), if one was involved;
- the command you ran;
- what `hi` printed, with the request id (`req_...`) if it showed one.

Issues are public. Never paste an API key, a sign-in token, a prompt, a model's answer or the contents of your files. A request id is enough for HIPS to find the request, whose record never holds its content.

The source of `hi` is not public, so this repository takes no pull requests. If you have a fix in mind, describe it in the issue.

## Report a vulnerability

Never open a public issue for a security problem. Email security@hips.com, under HIPS's Vulnerability Disclosure Policy at https://hips.com/security. See [SECURITY.md](SECURITY.md).
