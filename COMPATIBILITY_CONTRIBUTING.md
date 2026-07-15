# Contributing to PCSX5 Game Compatibility

Thank you for contributing to the PCSX5 Game Compatibility database! This guide will help you submit accurate and useful compatibility reports.

## 📋 Before You Submit

### Prerequisites
- **PCSX5 version**: Test with the latest stable or nightly build
- **PS5 Firmware**: Note the firmware version you tested on
- **Game dump**: Use a legitimate game dump (disc or digital)
- **Hardware specs**: CPU, GPU, RAM for context

### Required Information
Every report must include:
- [ ] Game title and Title ID (e.g., `PPSA-XXXXX_00`)
- [ ] PCSX5 version/commit hash
- [ ] PS5 Firmware version
- [ ] Status label (see below)
- [ ] Your hardware specs (CPU, GPU, RAM)
- [ ] Settings used (resolution, upscaling, etc.)

## 🏷️ Status Definitions

| Status | Label | Criteria |
|--------|-------|----------|
| **Playable** | `status-playable` | Completable with minor/no issues; stable 30/60 FPS |
| **In-Game** | `status-ingame` | Reaches gameplay but has major issues (crashes, graphics, performance) |
| **Menus** | `status-menus` | Boots to main menu only; crashes/freezes before gameplay |
| **Boots** | `status-boots` | Shows logo/intro but crashes before menu |
| **Nothing** | `status-nothing` | Black screen, immediate crash, or fails to boot |

## 📝 How to Submit a Report

### Option 1: GitHub Issues (Recommended)
1. Check if an issue already exists for the game (search by Title ID)
2. If not, click **New Issue** → **Compatibility Report**
3. Fill out the template completely
4. Apply the appropriate status label
5. Add `compat-report` label
6. Submit!

### Option 2: Update Existing Report
1. Find the existing issue for the game
2. Comment with your findings
3. If status has changed, update the label
4. Add your hardware/config if different from OP

## 🎮 Testing Guidelines

### Standard Test Procedure
1. **Boot game** → Note boot time and any errors
2. **Navigate menus** → Test all accessible menus
3. **Enter gameplay** → Play for at least 10-15 minutes
4. **Test saves** → Save/load functionality
5. **Check graphics** → Look for artifacts, missing textures, lighting issues
6. **Monitor performance** → FPS, frametime stability
7. **Test audio** → Music, SFX, voice acting

### Settings to Test
- **Resolution**: Native, 1080p, 4K
- **Upscaling**: FSR, NIS, or none
- **Frame limit**: 30, 60, or uncapped
- **Graphics backend**: Vulkan (preferred), OpenGL

### What to Document
- ✅ What works perfectly
- ⚠️ Minor issues (graphical glitches, occasional stutter)
- ❌ Major issues (crashes, game-breaking bugs, unplayable performance)
- 🔧 Workarounds (specific settings, patches, workarounds)

## 🏷️ Labeling Guidelines

### Required Labels
- **Exactly one** status label (required)
- `compat-report` (required)

### Optional Labels
- `graphics-issues` - Visual artifacts, missing textures
- `audio-issues` - Missing/crackling audio
- `performance` - Low FPS, stuttering
- `crashes` - Random or reproducible crashes
- `save-issues` - Save/load problems
- `requires-patch` - Needs game-specific patch
- `firmware-specific` - Works only on specific FW
- `verified` - Confirmed by multiple testers

## 📸 Evidence Requirements

### Screenshots (Recommended)
- In-game gameplay (not just menus)
- Any graphical issues
- Settings used

### Logs (For Crashes/Issues)
- PCSX5 log file (`pcsx5.log`)
- Crash dumps if available
- Console output

## 🔄 Updating Reports

### When to Update
- New PCSX5 version improves/breaks compatibility
- You tested with different settings/hardware
- Found a workaround for a known issue
- Game receives a patch/DLC

### How to Update
1. Comment on the existing issue
2. Include: PCSX5 version, what changed, new status if applicable
3. Update labels if status changed
4. Add new evidence (screenshots, logs)

## 🤝 Community Guidelines

- **Be respectful** - Different hardware yields different results
- **Be accurate** - Don't guess; test and report facts
- **Be specific** - "Crashes" is less helpful than "Crashes at character select with Vulkan"
- **Credit sources** - If using someone else's findings, reference them
- **No piracy discussion** - Focus on emulation accuracy, not acquisition

## 📚 Resources

- [PCSX5 Official Website](https://pcsx5.net)
- [PCSX5 GitHub](https://github.com/PCSX5/PCSX5)
- [PS5 Title ID Database](https://www.psdevwiki.com/ps5/Title_ID)
- [PCSX5 Compatibility Spreadsheet (Community)](https://docs.google.com/spreadsheets/d/1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgvE2upms/edit)

## ❓ Questions?

Open a [Discussion](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/discussions) or ask in the [PCSX5 Discord](https://discord.gg/pcsx5).

---

*Thank you for helping improve PCSX5 compatibility tracking!*
