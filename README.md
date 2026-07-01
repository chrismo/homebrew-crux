# homebrew-crux

Homebrew tap for [**crux**](https://github.com/chrismo/rwx-tui) — a local TUI
for monitoring RWX runs with a better Flow dependency-graph viewer.

## Install

```sh
brew install chrismo/crux/crux
```

or:

```sh
brew tap chrismo/crux
brew install crux
```

Then:

```sh
crux            # run list (home)
crux --run <id> # open a run's flow graph
crux --version
```

## How this tap is maintained

`Casks/crux.rb` is **generated and committed automatically** by
[GoReleaser](https://goreleaser.com) from the
[crux release workflow](https://github.com/chrismo/rwx-tui/blob/main/.github/workflows/release.yml)
on each `vX.Y.Z` tag. Don't hand-edit it.

macOS binaries are unsigned; the cask strips the Gatekeeper quarantine attribute
on install so `crux` runs without a security prompt.
