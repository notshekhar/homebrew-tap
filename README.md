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
| macOS | Intel (`x64`) | ❌ — use the installer below |
| Linux | `x64` | ✅ |
| Linux | `arm64` | ✅ |

**Intel macs:** there's no prebuilt x86_64 bottle yet, so `brew install` exits with a
pointer to the direct installer:

```sh
curl -fsSL https://raw.githubusercontent.com/notshekhar/loop/main/install.sh | bash
```

**Windows** isn't served via Homebrew — use the [PowerShell installer](https://github.com/notshekhar/loop#install).

## How this stays current

`Formula/loop.rb` is **auto-generated on every release** by the `update-homebrew-tap`
job in [notshekhar/loop](https://github.com/notshekhar/loop)'s `release.yml`. It reads
the published `SHA256SUMS` and rewrites the formula's `version` + checksums, then
pushes here. Don't hand-edit the formula — changes are overwritten on the next tag.
