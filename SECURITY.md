# Security

This policy covers every public repository under
[github.com/MatterWaveAI](https://github.com/MatterWaveAI) that has no `SECURITY.md` of its own, and
the hosted MatterWave service.

## Reporting a vulnerability

Email **security@matterwave.ai**, or report it privately on GitHub: on the repository's
**Security** tab, choose **Report a vulnerability** (GitHub's private vulnerability reporting).
Do not open a public issue, discussion or pull request for anything that could be a
vulnerability, in a repository or in the hosted service.

Include what you found, how to reproduce it, and the version or commit. You will get an
acknowledgement within three working days and a decision on severity and a fix timeline within
ten. We ask that you give us reasonable time to fix before any disclosure, and we will credit you
in the release notes unless you prefer otherwise.

## Scope

- The code in the organization's public repositories: the SDKs, the clients (terminal, VS Code,
  desktop), the website and the libraries.
- The hosted service at `app.matterwave.ai`, `docs.matterwave.ai` and `matterwave.ai`, for
  reports found by ordinary use. Please do not run automated scanners, load tests or
  denial-of-service attempts against the service, and do not access data that is not yours.

## Supported versions

The latest release of each SDK, client and library. Older versions receive fixes at our
discretion.
