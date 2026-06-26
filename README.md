# Retrace Homebrew tap

The official [Homebrew](https://brew.sh) tap for the **Retrace CLI** — record, replay, fork, and
manage AI agent traces from your terminal. Works on macOS, Linux, and WSL.

## Install

```bash
brew install --cask retraceai-tech/tap/retrace
```

That single command taps this repository and installs the CLI. On Homebrew 6.0+, the fully-qualified
`--cask` form is trust-exempt, so no separate `brew tap` / `brew trust` step is needed.

## Upgrade

```bash
brew upgrade --cask retrace
```

## Uninstall

```bash
brew uninstall --cask retrace
```

## How it works

The cask in [`Casks/retrace.rb`](Casks/retrace.rb) downloads the prebuilt binary for your platform
from the Retrace CDN (`cdn.retraceai.tech`) — the same artifacts used by the
`curl -fsSL https://retraceai.tech/install.sh | sh` installer and `retrace update`.

The cask is **auto-generated** by the Retrace CLI release pipeline on every new version; do not edit
`Casks/retrace.rb` by hand.

## Other install methods

```bash
# Install script (macOS, Linux, Windows)
curl -fsSL https://retraceai.tech/install.sh | sh
```

See the [CLI documentation](https://cli.retraceai.tech/docs/installation) for direct binary
downloads and all options.
