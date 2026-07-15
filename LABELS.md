# PCSX5 Game Compatibility - GitHub Labels Configuration
# This file documents the labels used for compatibility tracking
# Apply these labels in your GitHub repository settings

## 📊 Compatibility Status Labels (Mutually Exclusive - Use Exactly One)

| Label | Color | Description |
|-------|-------|-------------|
| `status-playable` | `#0e8a16` | **Playable** - Completable with minor/no issues; stable 30/60 FPS |
| `status-ingame` | `#fbca04` | **In-Game** - Reaches gameplay but has major issues (crashes, graphics, performance) |
| `status-menus` | `#d4c5f9` | **Menus** - Boots to main menu only; crashes/freezes before gameplay |
| `status-boots` | `#5319e7` | **Boots** - Shows logo/intro but crashes before menu |
| `status-nothing` | `#e99695` | **Nothing** - Black screen, immediate crash, or fails to boot |

## 🏷️ Required Labels

| Label | Color | Description |
|-------|-------|-------------|
| `compat-report` | `#0052cc` | **Required** - Marks issue as a compatibility report |

## 🔍 Issue Category Labels (Optional - Add as Applicable)

| Label | Color | Description |
|-------|-------|-------------|
| `graphics-issues` | `#d93f0b` | Visual artifacts, missing textures, lighting issues |
| `audio-issues` | `#bfd4f2` | Missing/crackling audio, no sound |
| `performance` | `#f9d0c4` | Low FPS, stuttering, frametime spikes |
| `crashes` | `#b60205` | Random or reproducible crashes |
| `save-issues` | `#c2e0c6` | Save/load problems, corrupted saves |
| `requires-patch` | `#fef2c0` | Needs game-specific patch or workaround |
| `firmware-specific` | `#d4c5f9` | Works only on specific PS5 firmware |
| `verified` | `#0e8a16` | Confirmed by multiple testers |

## 🎮 Game Metadata Labels (Optional)

| Label | Color | Description |
|-------|-------|-------------|
| `region-us` | `#0052cc` | North America region |
| `region-eu` | `#006b75` | Europe region |
| `region-jp` | `#d93f0b` | Japan region |
| `region-asia` | `#fbca04` | Asia region (HK, KR, TW) |
| `disc` | `#5319e7` | Physical disc version |
| `digital` | `#0052cc` | Digital download version |
| `dlc-tested` | `#bfd4f2` | DLC content tested |
| `update-tested` | `#c2e0c6` | Game update/patch tested |

## 🖥️ Platform Labels (Optional)

| Label | Color | Description |
|-------|-------|-------------|
| `platform-windows` | `#0078d4` | Tested on Windows |
| `platform-linux` | `#fcc624` | Tested on Linux |
| `platform-macos` | `#999999` | Tested on macOS |

## 📋 How to Apply Labels

### Via GitHub Web UI:
1. Open the issue
2. Click **Labels** in the right sidebar
3. Search/select the appropriate labels
4. **Important**: Only ONE status label per issue!

### Via GitHub CLI:
```bash
# Add status label (choose one)
gh issue edit 123 --add-label "status-playable"
gh issue edit 123 --add-label "status-ingame"
gh issue edit 123 --add-label "status-menus"
gh issue edit 123 --add-label "status-boots"
gh issue edit 123 --add-label "status-nothing"

# Add required label
gh issue edit 123 --add-label "compat-report"

# Add optional category labels
gh issue edit 123 --add-label "graphics-issues,performance,verified"
```

### Via GitHub API:
```bash
curl -X POST \
  -H "Authorization: token YOUR_TOKEN" \
  -H "Accept: application/vnd.github.v3+json" \
  https://api.github.com/repos/OWNER/REPO/issues/123/labels \
  -d '{"labels":["status-playable","compat-report","verified"]}'
```

## 🎨 Creating Labels in Repository Settings

Go to **Settings → Labels** and create each label with the specified color codes.

### Bulk Create via GitHub CLI:
```bash
# Status labels
gh label create "status-playable" --color "0e8a16" --description "Playable - Completable with minor/no issues"
gh label create "status-ingame" --color "fbca04" --description "In-Game - Reaches gameplay but has major issues"
gh label create "status-menus" --color "d4c5f9" --description "Menus - Boots to main menu only"
gh label create "status-boots" --color "5319e7" --description "Boots - Shows logo/intro but crashes before menu"
gh label create "status-nothing" --color "e99695" --description "Nothing - Black screen, immediate crash, or fails to boot"

# Required label
gh label create "compat-report" --color "0052cc" --description "Compatibility report issue"

# Category labels
gh label create "graphics-issues" --color "d93f0b" --description "Visual artifacts, missing textures, lighting issues"
gh label create "audio-issues" --color "bfd4f2" --description "Missing/crackling audio, no sound"
gh label create "performance" --color "f9d0c4" --description "Low FPS, stuttering, frametime spikes"
gh label create "crashes" --color "b60205" --description "Random or reproducible crashes"
gh label create "save-issues" --color "c2e0c6" --description "Save/load problems, corrupted saves"
gh label create "requires-patch" --color "fef2c0" --description "Needs game-specific patch or workaround"
gh label create "firmware-specific" --color "d4c5f9" --description "Works only on specific PS5 firmware"
gh label create "verified" --color "0e8a16" --description "Confirmed by multiple testers"
```

## 📝 Label Usage Rules

1. **Exactly ONE status label** per issue (required)
2. **`compat-report` label** required on all compatibility issues
3. Category labels are **optional** - add as many as apply
4. Region/platform labels are **optional** - add if known
5. `verified` label should only be added by maintainers after confirmation
6. Update status label when compatibility changes (new PCSX5 version, patches, etc.)

## 🔄 Label Maintenance

- Review labels quarterly
- Archive unused labels
- Keep color scheme consistent
- Document any new labels here
