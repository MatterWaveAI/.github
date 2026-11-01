# Contributing

Thank you. A few things make a change easy to take.

## Before you start

- **Bugs and small fixes**: open an issue or a pull request straight away.
- **Larger changes**: open an issue first and say what you have in mind, so the work is not
  wasted on something that will not be merged.
- **Each project lives in its own repository** under
  [github.com/MatterWaveAI](https://github.com/MatterWaveAI) (`python-sdk`, `typescript-sdk`,
  `tui`, `vscode-extension`, `desktop` and the libraries); open issues and pull requests in the
  one the change belongs to.
- **Security problems** never go in an issue: see [SECURITY.md](SECURITY.md).
- Everyone taking part follows the [code of conduct](CODE_OF_CONDUCT.md).

## Branches

- **`develop` is the branch to target.** Branch from `develop` and open the pull request against
  it. `main` is for releases; a pull request opened against `main` is retargeted to `develop`.
- Keep the branch up to date with `develop` before asking for review.

## Working on a repository

Each repository's README says how to set it up and which checks its CI runs. Run them before you
push.

Where a repository commits a lockfile (`uv.lock`, `pnpm-lock.yaml`, `Cargo.lock`), it is the
contract: install from it (`uv sync --locked`, `pnpm install --frozen-lockfile`) and commit it
with any dependency change.

## Pull requests

- **CI must be green.** A pull request with a failing check is not reviewed or merged until it
  passes.
- One concern per pull request, with a title that says what changes in plain words.
- Say what changed and why in the description; a reviewer should not need to read the diff to
  know what they are looking at.
- Add or change tests with the code they cover.
- Keep the README and the docs in step with the code they describe, and where the repository
  keeps a `CHANGELOG.md`, add the change under **Unreleased**.
- By submitting a contribution you agree it is licensed under the repository's licence (its
  `LICENSE` file); for the Apache License 2.0, that is what section 5 of the licence says.

## Style

Follow the formatter and linter the repository's CI runs. Write comments for the why, not the
what.
