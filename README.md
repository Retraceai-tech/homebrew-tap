# Retrace Homebrew tap

The official [Homebrew](https://brew.sh) tap for the **Retrace CLI** — record, replay, fork, and
manage AI agent traces from your terminal. Works on macOS, Linux, and WSL.

```bash
brew install --cask retraceai-tech/tap/retrace-cli
```

Upgrade with `brew upgrade --cask retrace-cli`, uninstall with `brew uninstall --cask retrace-cli`.

The cask in `Casks/retrace-cli.rb` is **auto-generated** by the Retrace CLI release pipeline on every
new version (do not edit it by hand) and downloads the prebuilt binary for your platform from the
Retrace CDN — the same artifacts used by `curl -fsSL https://retraceai.tech/install.sh | sh`.
