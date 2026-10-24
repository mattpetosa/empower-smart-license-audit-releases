# Release history

Newest first. Downloads are on the [Releases](https://github.com/mattpetosa/empower-smart-license-audit-releases/releases) page.

## v3.10.0.1-0.6.0 (2026-10-23)

### Fixed
- **Updates install from any folder.** An update could not install, and the app then closed each time it was started, when the app or the Windows user's folder had a curly apostrophe in its name (e.g. Matt’s tools). Folders with square brackets in their name (e.g. Tools [v2]) also restart correctly after an update now.
- **A stalled update download no longer hangs the app.** If the connection went quiet partway through downloading an update, the update window stayed open and the update button stayed disabled until the app was closed. The download now gives up after a minute without data.
- **The app opens even if an update file is busy.** If an antivirus scan was holding a downloaded update when the app started, the app closed straight away; it now opens normally and installs the update on a later start.
- **Last sign-in dates on servers with day-first dates.** Where Empower reports a last sign-in as text, dates such as 03/04/2026 are now read the way the server writes them (3 April on a UK or German server), not always month-first.
- **Long company names no longer block saving the audit file.** A very long company or database name made the file name too long for Windows, and the save form asked again and again.
- **Clearer message for a closed audit.** When your audit code belongs to an audit that is no longer taking uploads, the save form now says so instead of "No audit code was given".
- Log files use the same date and time format on every computer, whatever its regional settings.

## v3.10.0.1-0.5.3 (2026-10-08)

### Fixed
- **The ring on the running step turns.** Since 0.5.0 it stood still on many computers while a step ran. It now turns once a second for as long as the step runs.
- **The window stays responsive while a step runs.** Each step does its work in the background, so the window can be moved and Cancel answers straight away while a step is busy.

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
