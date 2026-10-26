# Higurashi Korean Patch Installer (macOS)

macOS installer for the Korean language patch of *Higurashi When They Cry* —
Ch.1–Ch.8, Rei and Hou+.

One command detects your Steam library, downloads only the files your installation
needs, verifies them, and applies the patch with backup and rollback.

```bash
curl -fsSL https://github.com/s485lee/Higurashi_Korean_Mac_Releases/releases/latest/download/install.sh | bash
```

> **Status: under construction.** The instructions above describe the planned
> installer and are not functional yet. Until the first release, use the existing
> per-chapter patch DMGs.

## What it will do

- Detect every supported title across all Steam libraries, including external drives
- Compose each install from three pinned sources: 07th-mod media → Korean overlay → Korean text
- Download only what changed (a text fix is a few KB, not a 2 GB DMG)
- Show real byte-level progress, verify every file, and keep a rollback
- Detect when a Steam update removed the patch and offer to re-apply it

## Requirements

- macOS 12 or later (Apple Silicon or Intel)
- A Steam installation of the game (GOG / MangaGamer builds are detected manually)

## Credits

- 07th-Mod — voice/graphics media and the upstream patch structure
- **s485lee** — macOS port and Korean patch maintenance
- **yuulafe** — Korean translation updates

The installer downloads 07th-Mod's media directly from their releases rather than
redistributing it.
