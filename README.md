# notshekhar/homebrew-tap

Homebrew tap for [`loop`](https://github.com/notshekhar/loop) — a terminal coding agent (multi-provider, fast, native TUI).

## Install

```sh
brew install notshekhar/tap/loop
```

That one command taps this repo and installs `loop` in a single step. After the first install you can drop the prefix:

```sh
brew install loop      # bare name works once the tap is added
brew upgrade loop
brew uninstall loop
```

Both `loop` and `agent` are placed on your `PATH`.

## Supported platforms

| Platform | Arch | Bottled |
| --- | --- | --- |
| macOS | Apple Silicon (`arm64`) | ✅ |
| macOS | Intel (`x64`) | ✅ from v0.5.6+ |
| Linux | `x64` | ✅ |
| Linux | `arm64` | ✅ |

Windows isn't served via Homebrew — use the [PowerShell installer](https://github.com/notshekhar/loop#install).

## How this stays current

`Formula/loop.rb` is **auto-generated on every release** by the `update-homebrew-tap`
job in [notshekhar/loop](https://github.com/notshekhar/loop)'s `release.yml`. It reads
the published `SHA256SUMS` and rewrites the formula's `version` + checksums, then
pushes here. Don't hand-edit the formula — changes are overwritten on the next tag.
