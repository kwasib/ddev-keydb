[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/kwasib/ddev-keydb/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/kwasib/ddev-keydb/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/kwasib/ddev-keydb)](https://github.com/kwasib/ddev-keydb/commits)
[![release](https://img.shields.io/github/v/release/kwasib/ddev-keydb)](https://github.com/kwasib/ddev-keydb/releases/latest)

# DDEV Keydb

## Overview

This add-on integrates Keydb into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get kwasib/ddev-keydb
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Keydb |
| `ddev logs -s keydb` | Check Keydb logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.keydb --keydb-docker-image="busybox:stable"
ddev add-on get kwasib/ddev-keydb
ddev restart
```

Make sure to commit the `.ddev/.env.keydb` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `KEYDB_DOCKER_IMAGE` | `--keydb-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@kwasib](https://github.com/kwasib)**
