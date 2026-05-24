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

- Resident always-on-top widget, on by default: the app runs as a widget that stays on screen instead of dismissing (set `widget_mode: false` for the classic tray-icon popup)
- Compact view with click-to-expand, drag-to-move, and a remembered window position (restored next launch; off-screen coordinates are auto-corrected; the first run opens centered)
- Right-click widget menu: always-on-top toggle, settings, about, quit
- Settings window to choose which usage fields are shown - per field show / collapse (hidden in the compact view, shown when expanded) / hide - with drag-to-reorder
- Language selector in the settings window (system default plus all 13 languages)
- About dialog with clickable links (a native Win32 task dialog)
- `widget_hide_account` setting to hide the account row in the widget
- `light_taskbar` setting to choose the tray icon glyph color (replaces the removed registry-based theme detection)

### Changed

- Renamed to "Claude Usage Monitor"; the executable is `ClaudeUsageMonitor.exe`
- Settings and widget state are stored in `ClaudeUsageMonitor.ini` next to the executable; the app no longer uses the Windows Registry
- Autostart ("Start with Windows") now uses a Startup-folder shortcut instead of a registry entry
- The widget UI (right-click menu, settings window, about dialog) is fully localized across all 13 languages

[Show all code changes](https://github.com/omi-last-stand/claude-usage-monitor/releases/tag/v1.0.0)
