# Zendrix Monthly Release Workflow

## Overview
This repository demonstrates a **Gitflow-based workflow** designed for Zendrix Softwares to manage **monthly product releases**. The workflow ensures that the `main` branch always contains production-ready code, while features are developed and tested in isolated branches before the monthly release.

## Branch Structure
- `main` – Production-ready code, updated only on release day (25th of each month)
- `develop` – Integration branch for all completed features
- `feature/*` – Feature branches for new development
- `release/*` – Branch created a few days before the 25th for final testing and release prep

## Workflow Steps
1. Create feature branches for each new feature.
2. Merge completed features into `develop`.
3. Create a `release/vYYYYMM` branch from `develop` before the 25th.
4. Perform final testing and fixes on the release branch.
5. Merge release branch into `main` on the 25th.
6. Merge release branch back into `develop` to keep it up-to-date.

## Notes
- Hotfixes are optional and can be created from `main` if critical bugs appear between releases.
- Tags are applied to `main` for every release (e.g., `v202508`).

## File Structure Example
