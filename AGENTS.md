# AGENTS.md — lab-series

## Project summary

Umbrella repository for nlink-jp's experimental projects under active
development; projects that mature graduate to a production series. Each
project lives in its own repository, included here as a submodule. The
catalog — one row per project — is [README.md](README.md); this file covers
only how to work with the umbrella (ADR-005).

## Key commands

| Command | Purpose |
|---------|---------|
| `git clone --recurse-submodules https://github.com/nlink-jp/lab-series.git` | Clone with all projects |
| `git submodule update --init` | Populate submodules in an existing clone |
| `git submodule update --remote <project>` | Pull a project's latest main |
| `git add <project>` → commit `chore: bump <project> to vX.Y.Z` | Update the pointer after a release |

## Gotchas

- Development happens in the project repositories; new projects start in
  the workspace root `_wip/`, never directly inside this umbrella
  (CONVENTIONS.md — Starting a New Project).
- Submodule checkouts default to detached HEAD — `git checkout main` inside
  a submodule before committing.
- Submodule URLs are HTTPS only (SSH fails on machines without key auth).
- Every submodule needs a catalog row in README.md — `check-org.sh` fails
  otherwise. When a project graduates to another series, keep its row only
  with an explicit label pointing at the new home.

## Module path

Repository: `github.com/nlink-jp/lab-series`
