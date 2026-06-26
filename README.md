<div align="center">

<img src="assets/banner.gif" alt="Retrace" width="480" />

![Homebrew](https://img.shields.io/badge/Homebrew-FBB040?logo=homebrew&logoColor=black)
![macOS](https://img.shields.io/badge/macOS-000000?logo=apple&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![WSL](https://img.shields.io/badge/WSL-4D4D4D?logo=windows&logoColor=white)

**The official Homebrew tap for the Retrace CLI.**

Record, replay, fork, and manage AI agent traces from your terminal — installable on macOS, Linux, and WSL.

[Retrace](https://retraceai.tech) · [CLI site](https://cli.retraceai.tech) · [Documentation](https://docs.retraceai.tech)

</div>

---

## Install

```bash
brew install --cask retraceai-tech/tap/retrace-cli
```

On Homebrew 6.0+ the fully-qualified `--cask` form taps and trusts this repository automatically — no separate `brew tap` / `brew trust` step. The CLI installs as the `retrace` command.

```bash
brew upgrade --cask retrace-cli      # update
brew uninstall --cask retrace-cli    # remove
```

> The cask token is `retrace-cli` (the command is still `retrace`) to avoid a collision with an unrelated `retrace` app in homebrew-cask.

## How it works

The cask in [`Casks/retrace-cli.rb`](Casks/retrace-cli.rb) downloads the prebuilt binary for your platform from the Retrace CDN (`cdn.retraceai.tech`) — the same artifacts used by the `curl -fsSL https://retraceai.tech/install.sh | sh` installer and `retrace update`.

It is **auto-generated** by the Retrace CLI release pipeline on every new version (do not edit it by hand).

## Other install methods

```bash
# Install script (macOS, Linux, Windows)
curl -fsSL https://retraceai.tech/install.sh | sh
```

See the [CLI documentation](https://cli.retraceai.tech/docs/installation) for direct binary downloads and all options.

## License

MIT — part of [Retrace](https://retraceai.tech), the execution replay engine for AI agents.
