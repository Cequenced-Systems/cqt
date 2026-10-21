# cqt

`cqt` is the Cequenced Team CLI: a terminal coding agent that talks to
OpenAI-compatible, Gemini and Anthropic providers, runs built-in and MCP
tools, and works with Cequenced Team accounts. It is one static binary with
no runtime to install.

## Install

Each [release](https://github.com/Cequenced-Systems/cqt/releases) has one
archive per OS and architecture (`amd64`, `arm64`):

- Linux: `cqt-<version>-linux-<arch>.tar.xz`
- Windows: `cqt-<version>-windows-<arch>.zip`

Each archive holds the `cqt` binary (`cqt.exe` on Windows), this README,
`LICENSE` and `licenses.txt`. `SHA256SUMS` covers every file.

```sh
tar -xJf cqt-v26.10.21.1-linux-amd64.tar.xz
sha256sum --ignore-missing -c SHA256SUMS
install -m 0755 cqt ~/.local/bin/cqt
cqt version
```

On Windows, unzip the archive and put `cqt.exe` somewhere on your `PATH`.
The Windows binaries are signed by Cequenced Systems, LLC.

## SBOMs

[SBOM/](SBOM) holds a CycloneDX SBOM for every binary,
`SBOM/<version>/cqt-<version>-<os>-<arch>.cdx.json`, listing the modules
linked into it and their licences. `licenses.txt` summarises them.

## First run

Run `cqt` and pick a provider, then a model; the choice is saved to
`~/.cqt/config.toml`. `cqt help` lists the commands and flags.

## Licence

cqt is proprietary; see [LICENSE](LICENSE).
