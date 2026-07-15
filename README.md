# PCSX5 Game Compatibility

[![GitHub Issues](https://img.shields.io/github/issues/Abhishekrazy/Pcsx5-Game-Compatibility?label=Total%20Reports&color=blue)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues)
[![GitHub Issues - Playable](https://img.shields.io/github/issues/Abhishekrazy/Pcsx5-Game-Compatibility/label/status-playable?label=Playable&color=0e8a16)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues?q=label%3Astatus-playable)
[![GitHub Issues - In-Game](https://img.shields.io/github/issues/Abhishekrazy/Pcsx5-Game-Compatibility/label/status-ingame?label=In-Game&color=fbca04)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues?q=label%3Astatus-ingame)
[![GitHub Issues - Menus](https://img.shields.io/github/issues/Abhishekrazy/Pcsx5-Game-Compatibility/label/status-menus?label=Menus&color=f9d0c4)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues?q=label%3Astatus-menus)
[![GitHub Issues - Boots](https://img.shields.io/github/issues/Abhishekrazy/Pcsx5-Game-Compatibility/label/status-boots?label=Boots&color=d4c5f9)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues?q=label%3Astatus-boots)
[![GitHub Issues - Nothing](https://img.shields.io/github/issues/Abhishekrazy/Pcsx5-Game-Compatibility/label/status-nothing?label=Nothing&color=ededed)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues?q=label%3Astatus-nothing)

[![GitHub Stars](https://img.shields.io/github/stars/Abhishekrazy/Pcsx5-Game-Compatibility?style=social)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/Abhishekrazy/Pcsx5-Game-Compatibility?style=social)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/forks)
[![GitHub Watchers](https://img.shields.io/github/watchers/Abhishekrazy/Pcsx5-Game-Compatibility?style=social)](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/watchers)

---

A community-driven compatibility database for **PCSX5** — the experimental PlayStation 5 emulator for Windows.

Track which games boot, which reach menus, which are playable, and what issues remain. Inspired by the excellent [shadPS4 Game Compatibility](https://github.com/shadps4-compatibility/shadps4-game-compatibility) project, built with modern GitHub features.

## 🎮 Quick Links

| Resource | Link |
|----------|------|
| **Submit a Report** | [New Issue](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues/new/choose) |
| **Browse All Reports** | [Issues](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues) |
| **Playable Games** | [label:status-playable](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues?q=label%3Astatus-playable) |
| **In-Game** | [label:status-ingame](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/issues?q=label%3Astatus-ingame) |
| **PCSX5 Emulator** | [github.com/PCSX5/PCSX5](https://github.com/Abhishekrazy/pcsx5) |
| **PCSX5 Discord** | [discord.gg/pcsx5](https://discord.gg/pcsx5) |
| **Download Latest Build** | [PCSX5 Releases](https://github.com/Abhishekrazy/pcsx5/releases) |

---

## 📊 Compatibility Statistics

<!-- AUTO-GENERATED: This table is updated via GitHub Actions -->

| Status | Count | Percentage |
|--------|-------|------------|
| ![Playable](https://img.shields.io/badge/Playable-0-0e8a16?style=flat-square) | 0 | 0% |
| ![In-Game](https://img.shields.io/badge/In--Game-0-fbca04?style=flat-square) | 0 | 0% |
| ![Menus](https://img.shields.io/badge/Menus-0-f9d0c4?style=flat-square) | 0 | 0% |
| ![Boots](https://img.shields.io/badge/Boots-0-d4c5f9?style=flat-square) | 0 | 0% |
| ![Nothing](https://img.shields.io/badge/Nothing-60-ededed?style=flat-square) | 60 | 100% |
| **Total** | **60** | **100%** |

> 📈 *Last updated: 2026-07-16 • [Refresh stats](https://github.com/Abhishekrazy/Pcsx5-Game-Compatibility/actions/workflows/update-stats.yml)*

---

## 🏷️ Status Definitions

| Label | Status | Criteria |
|-------|--------|----------|
| `status-playable` | **Playable** | Completable start-to-finish; minor graphical/audio issues OK; stable 30+ FPS |
| `status-ingame` | **In-Game** | Reaches gameplay but has major issues: crashes, severe glitches, unplayable performance, game-breaking bugs |
| `status-menus` | **Menus** | Boots to main menu/UI but cannot start actual gameplay (crashes on load, infinite loading, etc.) |
| `status-boots` | **Boots** | Shows console logo, developer intro, or brief video then crashes/hangs before menu |
| `status-nothing` | **Nothing** | Black screen, immediate crash, or "not supported" error |

---

## 📝 How to Submit a Report

### Prerequisites
- Test with the **latest PCSX5 release** or recent main branch build
- Use **unmodified game dumps** from your own legally owned discs
- Dump **PS5 firmware modules** from your own console (required for most games)

### Step-by-Step

1. **Check existing issues** — Search for the game's Title ID (e.g., `CUSA00001`) to avoid duplicates
2. **Open a new issue** — Use the **"Compatibility Report"** template
3. **Fill in all fields** — The template includes a checklist and all required metadata
4. **Add evidence** — Screenshots, videos, and log snippets help developers immensely
5. **Submit** — Maintainers will review and apply the appropriate status label

### Report Template Preview

```markdown
## Game Information
- **Game Name:** [e.g., Astro's Playroom]
- **Title ID:** [e.g., CUSA00001]
- **Game Version:** [e.g., v1.00]
- **Region:** [e.g., US/EU/JP]
- **PlayStation Store URL:** [optional]

## Test Environment
- **PCSX5 Version/Commit:** [e.g., v0.1.0 / a1b2c3d]
- **Operating System:** [Windows 11 23H2 / Ubuntu 24.04 / macOS 14]
- **CPU:** [e.g., Ryzen 7 7800X3D]
- **GPU:** [e.g., RTX 4090 24GB]
- **RAM:** [e.g., 32GB DDR5-6000]

## Compatibility Status
- **Status:** [Playable / In-Game / Menus / Boots / Nothing]
- **FPS Range:** [e.g., 45-60 FPS]
- **Resolution Tested:** [e.g., 1920x1080]

## Issues Checklist
- [ ] Crashes / Freezes
- [ ] Graphical Glitches
- [ ] Audio Issues
- [ ] Input / Controller Problems
- [ ] Performance Issues
- [ ] Missing Features (trophies, saves, etc.)
- [ ] Requires Specific Settings
- [ ] Other: ___________

## Additional Notes
- **Error Messages/Logs:** [paste relevant log snippets]
- **Workarounds:** [any settings that help]
- **Screenshots/Videos:** [drag & drop or link]
```

---

## 🔧 Required Firmware Files

PCSX5 requires PS5 system modules (firmware) to run games. **You must dump these from your own PS5 console.**

| File | Description |
|------|-------------|
| `libkernel.sprx` | Kernel syscall interface |
| `libc.sprx` | C standard library |
| `libm.sprx` | Math library |
| `libSceAudio*.sprx` | Audio system modules |
| `libSceVideoOut*.sprx` | Video output modules |
| `libScePad*.sprx` | Controller input modules |
| `libSceGnm*.sprx` | Graphics API (GNM) modules |
| ...and more | See [PCSX5 docs](https://github.com/PCSX5/PCSX5/wiki/Firmware) for full list |

> ⚠️ **Legal:** Do not download firmware from the internet. Dump from your own console. Sharing Sony's proprietary firmware is illegal.

---

## 🧪 Testing Best Practices

### Baseline Settings for Consistent Reports
```ini
[Graphics]
Backend = Vulkan
Resolution = Native (1920x1080)
VSync = Disabled
Upscaling = None

[CPU]
Recompiler = LLVM
Thread Count = Auto

[Audio]
Backend = Default
Sample Rate = 48000
```

### What to Test
- [ ] Cold boot from game list
- [ ] Main menu navigation
- [ ] New game / Continue
- [ ] First 15-30 minutes of gameplay
- [ ] Save / Load functionality
- [ ] Video playback (cutscenes)
- [ ] Audio (music, SFX, voice)
- [ ] Controller input (all buttons, sticks, triggers)
- [ ] Sleep/Resume (if applicable)

---

## 🤝 Contributing

### Ways to Help
- 🎮 **Test games** and submit reports
- 🔄 **Update existing reports** with new findings or regressions
- 📝 **Improve documentation** — fix typos, add missing info
- 🤖 **Automation** — enhance issue creation scripts, stats generation
- 🏷️ **Triage** — help label and organize issues

### Guidelines
- **One game per issue** — Title format: `[CUSA00001] Game Name`
- **Be specific** — Include exact PCSX5 commit, game version, and settings
- **Evidence matters** — Screenshots, videos, logs accelerate fixes
- **Report regressions** — If a game breaks in a newer build, comment on the issue

### Labels Reference

| Category | Labels |
|----------|--------|
| **Status** | `status-playable`, `status-ingame`, `status-menus`, `status-boots`, `status-nothing` |
| **Type** | `compat-report`, `regression`, `needs-retest` |
| **Component** | `graphics`, `audio`, `input`, `performance`, `firmware-issue`, `cpu`, `memory` |
| **Platform** | `windows`, `linux`, `macos` |

---

## 🔗 Related Projects

| Project | Description |
|---------|-------------|
| **[PCSX5](https://github.com/PCSX5/PCSX5)** | Main emulator repository |
| **[PCSX5-QtLauncher](https://github.com/PCSX5/PCSX5-QtLauncher)** | Official GUI launcher |
| **[shadPS4 Compatibility](https://github.com/shadps4-compatibility/shadps4-game-compatibility)** | PS4 compatibility reference |
| **[RPCS3 Compatibility](https://github.com/RPCS3/compatibility)** | PS3 compatibility database |

---

## 📜 License

This compatibility database is released under the **MIT License** — see [LICENSE](LICENSE) for details.

PCSX5 itself is licensed under **GPL-2.0-or-later**.

---

## ⭐ Support

If you find this database useful:

- ⭐ **Star this repo** — helps others discover it
- 🐛 **Submit reports** — every game tested grows the database
- 💬 **Join the community** — [PCSX5 Discord](https://discord.gg/pcsx5)
- 💻 **Contribute to PCSX5** — code, docs, testing

---

<p align="center">
  <sub>Built with ❤️ by the PCSX5 community • Not affiliated with Sony Interactive Entertainment</sub>
</p>
