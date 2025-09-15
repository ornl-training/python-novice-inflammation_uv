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

## Obtain lesson materials

1. Download [python-novice-inflammation-data.zip][zipfile1]
  and [python-novice-inflammation-code.zip][zipfile2].
2. Create a folder called `swc-python` on your Desktop.
3. Move downloaded files to `swc-python`.
4. Unzip the files.

You should see two folders called `data` and `code` in the `swc-python` directory on your
Desktop.

## Launch Python interface

To start working with Python, we need to launch a program that will interpret and execute our
Python commands. For this workshop, we will assume the use of Jupyter Notebook.

## Jupyter Notebook

A Jupyter Notebook provides a browser-based interface for working with Python.
You can launch a notebook from the command line:

:::::::::::::::: spoiler

## Command line (Terminal)

1\. Navigate to the `data` directory:

::::::::::::::::: spoiler

## Unix shell

If you're using a Unix shell application, such as Terminal app in macOS, Console or Terminal
in Linux, or [Git Bash][gitbash] on Windows, execute the following command:

```bash
cd ~/Desktop/swc-python/data
```

:::::::::::::::::::::::::

::::::::::::::::: spoiler

## Command Prompt (Windows)

On Windows, you can use its native Command Prompt program.  The easiest way to start it up is
pressing <kbd>Windows Logo Key</kbd>\+<kbd>R</kbd>, entering `cmd`, and hitting
<kbd>Return</kbd>. In the Command Prompt, use the following command to navigate to
the `data` folder:

```source
cd /D %userprofile%\Desktop\swc-python\data
```

:::::::::::::::::::::::::

2\. Start Jupyter server

::::::::::::::::: spoiler

```bash
uv init
uv add jupyter matplotlib numpy
uv run jupyter notebook
```

If you run into errors, then try adding the `--native-tls` flag:

```bash
uv --native-tls init
uv --native-tls add jupyter matplotlib numpy
uv run jupyter notebook
```

:::::::::::::::::::::::::

3\. Launch the notebook by clicking on the "New" button on the right and selecting "Python 3"
from the drop-down menu:
![](fig/jupyter-notebook-launch-notebook2.png){alt='Anaconda Navigator Notebook directory'}

:::::::::::::::::::::::::

[zipfile1]: data/python-novice-inflammation-data.zip
[zipfile2]: ../episodes/files/code/python-novice-inflammation-code.zip