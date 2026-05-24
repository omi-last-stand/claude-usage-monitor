# Privacy Policy

**Claude Usage Monitor** is a local desktop application that monitors your Claude API usage.

## Data Collection

This application does **not** collect, store, or transmit any personal data.

## Network Communication

The application communicates exclusively with `api.anthropic.com` to retrieve your current API usage
data. No other network connections are made.

## Credentials

The application reads your existing Claude OAuth token from the local Claude CLI configuration file
(`~/.claude/.credentials.json`). This token is:

- Used solely in HTTP Authorization headers to authenticate with the Anthropic API
- Never logged, stored elsewhere, copied, or transmitted to any third party

## Local Storage

The application writes one file, `ClaudeUsageMonitor.ini`, in the same folder as the executable. It
stores only the widget's display state - window position, the always-on-top preference, and which
usage fields are shown - and never contains credentials, account details, or usage values.

If you enable "Start with Windows", the application also creates a shortcut in your Windows Startup
folder, and removes it when you disable the option. No Windows Registry keys are written.

Usage data itself is kept in memory only and discarded when the application closes. An optional,
user-provided settings file (`usage-monitor-settings.json`) is only ever read, never written.

## Third-Party Services

The application does not integrate with any analytics, tracking, advertising, or telemetry services.

## Contact

For questions about this privacy policy, please open an issue at
https://github.com/omi-last-stand/claude-usage-monitor/issues
