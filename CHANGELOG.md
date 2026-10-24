# Changelog

## 1.2.0

- **New look:** Trader+ Dark (default) with black workstation keys, green accent, bold Segoe UI labels and an animated icon for every key; Buy green and Sell red in every style. Trader+ Light, Colourful, Vivid and Pro share the icons.
- **Safety:** Custom shortcut and other non-trading keys refuse Enter and multi-key sequences in this trading app. Buy and Sell keep single-tap behaviour (Flatten and Cancel orders still need a 1-second hold).
- **Fixed:** after a trading-worker error the next press no longer fails with "starting".
- Non-trading shortcut keys use the faster background helper, which checks Trader+ is in front before each step.
- Installer: asks before installing Stream Deck, waits up to 60 s for startup, works when WMI is restricted, independent rollback steps, pinned package checksum.
- `npm test` now also runs the trading-input checks. Added a trading-risk notice; the README now reads as user documentation.

## 1.1.2

- Restored the original Unicode label separators and broker notes.
- Reject invalid UTF-8 in app configuration during builds.

## 1.1.1

- Added a double-click Windows installer with prerequisite checks, package verification, local backups, preserved profiles/settings and automatic rollback.
- Included the pinned Windows Daily Toolkit dependency for automatic app switching. Compatible or newer installed versions are kept.
- Added a connected-runtime startup receipt and isolated installer tests.
- Added installation, update, troubleshooting and recovery documentation.
- Switched the development bundler to official Rollup WASM for restricted Windows environments.
