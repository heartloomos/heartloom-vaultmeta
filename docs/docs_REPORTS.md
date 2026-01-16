# REPORTS

VaultMeta Phase 0 generates two **stable notes** (overwritten each run).

---

## Output directory

Reports are written to:

- `OUTPUT_DIR` from config

If `OUTPUT_DIR` is blank, VaultMeta offers:

- `$VAULT_ROOT/30_REFERENCE/vaultmeta/`

---

## Reports (Phase 0)

### 1) VaultMeta - File Tree.md

A readable bullet-tree of your vault (depth-limited), optionally including files.

Common uses:
- “What’s actually in my vault right now?”
- sanity-checking structure after reorganizations
- quick scanning for new / unexpected folders

### 2) VaultMeta - Directory Blocks.md

A list of directories as one fenced block per directory:

```bash
/path/to/dir
```

Common uses:
- copy/paste paths into Termux or a desktop shell
- quick navigation when scripting or moving content
- grabbing exact directory paths without manual typing

---

## Report headers

Each report includes:
- frontmatter properties (`type`, `title`, `generated`, `vault_root`, `output_dir`, `version`)
- a “Settings Summary” section showing effective config values

This makes reports self-describing when shared, copied, or viewed later.

---

## Stability contract

- These notes are **always overwritten** on each run.
- VaultMeta does not create “daily” files or accumulate history in Phase 0.
- Later phases may add optional diff/history features, but stable notes remain the core contract.
