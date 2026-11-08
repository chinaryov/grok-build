# RH-PATCHES

The patch ledger of `chinaryov/grok-build`, the ReviewHerd fork of
[`xai-org/grok-build`](https://github.com/xai-org/grok-build).
Branch `rh/main` is the upstream base plus the patches below. Nothing else.

Upstream base: 1.0.45 2bdd1d6a6369de0e8c68132ea4539e9abd9e14a8

The base line holds the upstream version (from
`crates/codegen/xai-grok-version/Cargo.toml`) and the full upstream `main`
commit. Upstream has no release tags, so the gate checks that the commit is on
upstream `main` and carries that version.

## Rules

- The gate (`.reviewherd.yaml`, check `ledger`) lists every file that differs
  from the base: `git diff --name-only --no-renames -z <base> HEAD`. Each one
  must be `RH-PATCHES.md`, `.reviewherd.yaml` or a file of a patch below.
- A patch section names each file it changes on its own line, as
  ``- file: `path/from/repo/root` ``.
- A sync with upstream merges the new upstream commit and bumps the base line
  in the same PR.

## Patches

None yet.
