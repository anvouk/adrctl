# adrctl

Custom-made little cli tool to handle markdown
[Architectural Decision Records (ADRs)](https://adr.github.io) inside your
project.

Based on [MADR format spec](https://adr.github.io/madr/)

## Usage

1. Open shell in your project
2. Run `adrctl init`
3. Create new ADR `adrctl new My awesome shining new feature`

This will create the file `0001-my-awesome-shining-new-feature.md` with the short
template inside.

You can list ADRs with `adrctl list`

Help message with `adrctl`

> **Note**: ADRs file numbering is automatically handled by the cli.

## Installation

### Linux/macOS

1. Download `adrctl`
2. Ensure it has execute permissions `chmod +x adrctl`
3. Move it to local bin (e.g. `sudo mv adrctl /usr/local/bin`)

### Windows

1. Install [WSL](https://learn.microsoft.com/en-us/windows/wsl/install)
2. Follow the Linux installation procedure above

## Requirements to run

- POSIX sh (dash is ok)
- POSIX common utilities (e.g. `sed`, `tr`, etc)

## Known limitations

- Grouping MADRs in Sub directories is not yet supported (though can be manually
targeted by setting `ADRCTL_ADR_FOLDER=docs/decisions/sub` before running `adctl`)
- Long version template is not provided

## TODO

- Grouping in sub folders
- Long version template support
- Basic sh completion

## License

Apache-2.0 license
