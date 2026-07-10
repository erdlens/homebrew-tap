# homebrew-tap

The [Homebrew](https://brew.sh) tap for [erdlens](https://github.com/erdlens/erdlens).

## Install

```sh
brew install erdlens/tap/erdlens
```

Then:

```sh
erdlens --help
```

## Upgrade

```sh
brew update
brew upgrade erdlens
```

## Uninstall

```sh
brew uninstall erdlens
brew untap erdlens/tap
```

## How this tap is maintained

Everything in this repo is **auto-generated**. On every tagged release of `erdlens/erdlens`, the [`release` workflow](https://github.com/erdlens/erdlens/blob/main/.github/workflows/release.yml) runs [GoReleaser](https://goreleaser.com), which:

1. Cross-compiles binaries for macOS + Linux (amd64 + arm64).
2. Uploads them as archives to the GitHub Release.
3. Commits an updated `Formula/erdlens.rb` here, pinned to the new version + SHA256 of each archive.

**Do not hand-edit `Formula/erdlens.rb`** — your changes will be overwritten on the next release. If something is wrong with the formula, fix the `brews:` section in [`.goreleaser.yaml`](https://github.com/erdlens/erdlens/blob/main/.goreleaser.yaml) in the main repo.

## Reporting issues

For install / brew-specific issues: open an issue here.
For everything else: open one on [erdlens/erdlens](https://github.com/erdlens/erdlens/issues).

## License

MIT — see [LICENSE](./LICENSE) in the [main erdlens repo](https://github.com/erdlens/erdlens/blob/main/LICENSE).
