---
title: Setup
---

## Overview

This lesson is designed to be run on a personal computer.
All of the software and data used in this lesson are freely available online,
and instructions on how to obtain them are provided below.

## Install uv and Python

You will need to install the uv tool for this workshop. Detailed training on uv is available [here](https://ornl-training.github.io/python-with-uv/). The below instructions are copied from that workshop.

Install uv on macOS and Linux with:

```bash
$ curl -LsSf https://astral.sh/uv/install.sh | sh
# If curl is not present, then you can try wget below
$ wget -qO- https://astral.sh/uv/install.sh | sh
```

Install uv on Windows with:

```bash
$ powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

You may need to restart your terminal to ensure that uv was installed. Check the installation by displaying the version number using the `--version` option as shown below. If the command displays the uv version number then the installation was successful.

```bash
$ uv --version
```

```output
uv 0.8.4 (e176e1714 2025-07-30)
```
