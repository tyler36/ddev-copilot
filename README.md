[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/tyler36/ddev-copilot/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/tyler36/ddev-copilot/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/tyler36/ddev-copilot)](https://github.com/tyler36/ddev-copilot/commits)
[![release](https://img.shields.io/github/v/release/tyler36/ddev-copilot)](https://github.com/tyler36/ddev-copilot/releases/latest)

# DDEV Copilot

## Overview

This add-on integrates Copilot into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get tyler36/ddev-copilot
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Copilot |
| `ddev logs -s copilot` | Check Copilot logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.copilot --copilot-docker-image="ddev/ddev-utilities:latest"
ddev add-on get tyler36/ddev-copilot
ddev restart
```

Make sure to commit the `.ddev/.env.copilot` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `COPILOT_DOCKER_IMAGE` | `--copilot-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@tyler36](https://github.com/tyler36)**
