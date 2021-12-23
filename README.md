# Ansible Execution Environment: Netbox Inventory

[![N|Solid](https://netbox.readthedocs.io/en/stable/netbox_logo.svg)](https://netbox.readthedocs.io/)

## Overview

This project aims to sync Netbox inventory into Ansible AWX through the construct of an Execution Environment.

### 🐍 Prep your Python environment

I have included a Poetry file for anyone saavy enough to take advantage. For the uninitiated, Poetry helps replicate Python environments between users with a single file. You'll need to have Poetry installed on your machine, for most users that will be solved with `pip install poetry`.

1. install Python dependencies

```bash
poetry install
```

2. activate environment

```bash
poetry shell
```

## Executing the build

build the container image with

```bash
ansible-builder build --tag (please insert the name of your container image here)
```

## Upload container image

Your last step will be to upload your resulting Docker container image to a centralized repository that Ansible AWX can access.

## 📝 Dependencies

Refer to the Poetry Lock file located at [poetry.lock](poetry.lock) for detailed descriptions on each package installed.
