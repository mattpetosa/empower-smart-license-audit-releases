# Release history

Newest first. Downloads are on the [Releases](https://github.com/mattpetosa/empower-smart-license-audit-releases/releases) page.

## v3.10.0.1-0.4.8 (2026-10-06)

### Changed
- **Check for app updates from the header.** A small round arrow button beside the version opens a window that shows each step as it happens: the check for a newer version, the download (verified before it's kept), and finally **Restart now** / **Later** — or "You have the latest version". After an update the version in the header reads "Updated to v…" in green for that session.

## v3.10.0.1-0.4.7 (2026-10-06)

### Changed
- **Logs and settings live under C:\Client**, like the other Smart Tools, in folders named for this app: `C:\Client\Logs\Empower Smart License Audit` and `C:\Client\Settings\Empower Smart License Audit` — both readable by administrators only (the settings folder remembers your audit code). Nothing is kept in ProgramData any more; logs and settings from earlier versions are moved over the first time the app opens.

