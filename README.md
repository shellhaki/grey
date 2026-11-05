# grey

The command line for [Greyship](https://greyship.tech): deploy Go backends that scale to zero.

## Install

```sh
curl -fsSL https://greyship.tech/install | sh
```

or straight from this repo:

```sh
curl -fsSL https://raw.githubusercontent.com/shellhaki/grey/main/install.sh | sh
```

macOS and Linux, Intel and ARM. On Windows, install it inside WSL. The installer checks the download's sha256
against `checksums.txt` and puts `grey` (and the aliases `gray` and `greyship`) in `/usr/local/bin`, or
`~/.local/bin` when that isn't writable. It never asks for sudo. Run it again to update.

Pick a version with `GREY_VERSION=v0.1.0`, or a folder with `GREY_INSTALL_DIR=~/bin`.

## Use

```sh
grey login        # opens the browser to sign in
cd my-go-project
grey deploy       # builds on your machine if Go is installed, otherwise on Greyship
grey logs -f
```

`grey --help` lists everything: env vars, rollbacks, GitHub deploys, notifications.

This repo only holds the installer and the releases.
