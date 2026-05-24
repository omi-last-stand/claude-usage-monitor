# Changelog

All notable changes to this fork (Claude Usage Monitor) are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

This is a fork of [Usage Monitor for Claude](https://github.com/jens-duttke/usage-monitor-for-claude)
by Jens Duttke. For the history before the fork, see the
[upstream changelog](https://github.com/jens-duttke/usage-monitor-for-claude/blob/main/CHANGELOG.md).

## [1.0.0] - 2026-05-24

First release of the fork, based on Usage Monitor for Claude (upstream v1.15.1).

### Added

- Resident always-on-top widget: the app runs as a widget that stays on screen instead of dismissing
- Compact view with click-to-expand and drag-to-move; the window position and the compact/expanded view are remembered and restored next launch (off-screen coordinates are auto-corrected; the first run opens centered and compact)
- Right-click widget menu: always-on-top toggle, settings, about, quit
- Settings window to choose which blocks are shown and in what order - the account row, each usage bar, the extra-usage bar, the Claude Code versions, and the status line - each with show / collapse (shown only when expanded) / hide and drag-to-reorder
- Language selector in the settings window (system default plus all 13 languages); the app restarts automatically to apply the new language
- About dialog with clickable links (a native Win32 task dialog)

### Changed

- Renamed to "Claude Usage Monitor"; the executable is `ClaudeUsageMonitor.exe`
- Widget state is stored in `ClaudeUsageMonitor.ini` next to the executable (optional advanced settings remain in `usage-monitor-settings.json`); the app no longer uses the Windows Registry
- Autostart ("Start with Windows") now uses a Startup-folder shortcut instead of a registry entry
- The widget UI (right-click menu, settings window, about dialog) is fully localized across all 13 languages
- The system-tray icon is a fixed brand mark (the resident widget shows live usage); upstream's dynamic gauge icon and its `icon_fields` / `light_taskbar` / `icon_light` / `icon_dark` settings were removed

[Show all code changes](https://github.com/omi-last-stand/claude-usage-monitor/releases/tag/v1.0.0)
