# Release history

Newest first. Downloads are on the [Releases](https://github.com/mattpetosa/empower-smart-license-audit-releases/releases) page.

## v3.10.0.1-0.5.3 (2026-10-08)

### Fixed
- **The ring on the running step turns.** Since 0.5.0 it stood still on many computers while a step ran. It now turns once a second for as long as the step runs.
- **The window stays responsive while a step runs.** Each step does its work in the background, so the window can be moved and Cancel answers straight away while a step is busy.

## v3.10.0.1-0.5.2 (2026-10-08)

### Fixed
- **The running step's ring turns smoothly, and the window stays responsive.** Each step now does its work in the background, so the ring keeps turning while the step runs — before, it froze or jumped while a step was busy — and the window can still be moved or cancelled.

## v3.10.0.1-0.5.1 (2026-10-08)

### Fixed
- **The running step's ring spins again.** On computers where Windows' window animations are turned off — Remote Desktop sessions and servers set for best performance — the ring on the running step stood still. It now always turns while a step is running.

## v3.10.0.1-0.5.0 (2026-10-08)

### Changed
- **A new look.** A header band shows the database being audited, the step you're on and progress across every step; a side panel shows this database, what was collected and which databases have been sent.
- **A refreshed step list.** Numbered steps, a spinning ring on the step that is running, and a progress bar that fills one segment per step.

## v3.10.0.1-0.4.8 (2026-10-06)

### Changed
- **Check for app updates from the header.** A small round arrow button beside the version opens a window that shows each step as it happens: the check for a newer version, the download (verified before it's kept), and finally **Restart now** / **Later** — or "You have the latest version". After an update the version in the header reads "Updated to v…" in green for that session.

## v3.10.0.1-0.4.7 (2026-10-06)

### Changed
- **Logs and settings live under C:\Client**, like the other Smart Tools, in folders named for this app: `C:\Client\Logs\Empower Smart License Audit` and `C:\Client\Settings\Empower Smart License Audit` — both readable by administrators only (the settings folder remembers your audit code). Nothing is kept in ProgramData any more; logs and settings from earlier versions are moved over the first time the app opens.

