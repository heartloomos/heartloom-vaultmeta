# INSTALL

## Install (Termux or desktop)

From repo root:

```sh
./install.sh install
```

Installs:
- `vaultmeta` into `~/.local/bin/vaultmeta`
- Creates `config/vaultmeta.conf` if missing (from example)
- Optionally installs Termux:Widget shortcut `run-vaultmeta` into `~/.shortcuts/`

### Termux shortcut behavior (integrity-safe)
- Detects Termux via `$PREFIX` or `termux-info`
- If you opt into shortcut creation but Termux shortcuts directory is missing (or not Termux), it will skip with:

“Skipping shortcut creation because Termux shortcut directory does not exist.”

## Status

```sh
./install.sh status
vaultmeta status
```

## Edit config

```sh
./install.sh edit-config
```

Uses `$EDITOR` when available, otherwise tries `nano`, then `vi`, then a minimal inline prompt.

## Uninstall

```sh
./install.sh uninstall
```

Uninstall never deletes your vault. It removes installed binary and shortcut.
It will ask before removing the config file.
