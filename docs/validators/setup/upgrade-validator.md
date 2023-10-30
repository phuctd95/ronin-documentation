---
description: Latest software for Ronin nodes.
title: Upgrade validator version
tags:
- decoupling
---

## Overview

This page describes how to get the latest version of the node's software.

## Ronin node

Every Ronin node release is published on
[GitHub](https://github.com/axieinfinity/ronin/releases).

### Mainnet

To find the Docker image for each mainnet release, visit the following:

* [GitHub Container Registry](https://github.com/axieinfinity/ronin/pkgs/container/ronin)

To download the latest image for your node, follow these steps:

1. In the `.env` file, set `NODE_IMAGE` to the following:

    ```
    ghcr.io/axieinfinity/ronin:v2.6.2-800ec03
    ```

2. Save the changes.
3. Run `docker-compose up -d`.

### Saigon testnet

To find the Docker image for each testnet release, visit
[Docker Hub](https://hub.docker.com/r/axieinfinity/ronin-testnet/tags).

To download the latest image for your node, follow these steps:

1. In the `.env` file, set `NODE_IMAGE` to the following:

    ```
    ghcr.io/axieinfinity/ronin:v2.6.0-83c8375
    ```

2. Save the changes.
3. Run `docker-compose up -d`.

## See also

* [Upgrade bridge operator version](./../../bridge-operators/setup/upgrade-bridge.md)