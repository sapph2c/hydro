# Hydro

![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fsapph2c%2Fhydro%2Fmain%2Fpyproject.toml&style=for-the-badge&logo=python&logoSize=auto)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/sapph2c/hydro/ci.yml?style=for-the-badge&logo=github&logoSize=auto)
![GitHub deployments](https://img.shields.io/github/deployments/sapph2c/hydro/pypi?style=for-the-badge&logo=pypi&logoColor=white&logoSize=auto)

Hydro is a MD5 hash cracker written in Python.

## Install

Hydro is available as a Python package on PyPI and can be installed using `uv` (recommended), `pipx`, or `pip`.

**Note**: python 3.13+ is required

Install using uv:

```bash
uv install tool hydro-cli@latest
```

Install using pipx:

```bash
pipx install hydro-cli
```

Install using pip:

```bash
pip install hydro-cli
```

## Usage

To crack a hash located within `hash.txt` with the `rockyou.txt` wordlist:

```bash
hydro hash.txt rockyou.txt
```

Sample output:

```bash
❯ uv run hydro hash.txt rockyou.txt

Success! 5f4dcc3b5aa765d61d8327deb882cf99:password
```
