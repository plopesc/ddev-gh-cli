[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/plopesc/ddev-gh-cli/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/plopesc/ddev-gh-cli/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/plopesc/ddev-gh-cli)](https://github.com/plopesc/ddev-gh-cli/commits)
[![release](https://img.shields.io/github/v/release/plopesc/ddev-gh-cli)](https://github.com/plopesc/ddev-gh-cli/releases/latest)

# DDEV GH CLI

## Overview

This add-on integrates GH CLI into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get plopesc/ddev-gh-cli
ddev restart
```

If your GitHub token is already stored in `~/.config/gh/hosts.yml`, no additional configuration is required. Otherwise, you must set either the `GH_TOKEN` or `GITHUB_TOKEN` environment variable with a valid token.

To retrieve your token, run the following command on your host machine:
```sh
gh auth token
```

## Usage

| Command                                     | Description                              |
|---------------------------------------------|------------------------------------------|
| `ddev exec gh --version`                    | Check the installed version              |
| `ddev exec gh --help`                       | View available commands                  |

The full documentation about GH CLI can be gound at the ]GH CLI documentation page](https://cli.github.com/).

## Credits

**Contributed and maintained by [@plopesc](https://github.com/plopesc)**
