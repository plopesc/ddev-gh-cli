[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/plopesc/ddev-gh/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/plopesc/ddev-gh/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/plopesc/ddev-gh)](https://github.com/plopesc/ddev-gh/commits)
[![release](https://img.shields.io/github/v/release/plopesc/ddev-gh)](https://github.com/plopesc/ddev-gh/releases/latest)

# DDEV Gh

## Overview

This add-on integrates Gh into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get plopesc/ddev-gh
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Gh |
| `ddev logs -s gh` | Check Gh logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.gh --gh-docker-image="ddev/ddev-utilities:latest"
ddev add-on get plopesc/ddev-gh
ddev restart
```

Make sure to commit the `.ddev/.env.gh` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `GH_DOCKER_IMAGE` | `--gh-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@plopesc](https://github.com/plopesc)**
