# Changelog

## 2.0.0

> [!WARNING]
> Back up your old files if you might want to go back to an older version. The storage format has
> changed, and older versions will lose a lot of data if you revert.

### License

- Repetier-Server is now free for everyone. All features are available without a license key.

### New

- Improved frontend design.
- Bambu Lab printers supported (beta).
- New webcam management supporting more webcam types and sources.
- Maintenance support.
- Per-printer notes for maintenance, to-dos or important information.
- Heightmap for Klipper.
- Named fans for Klipper.
- View printer and server logs in the user interface.
- Folders for G-code storage instead of groups.
- More computed expressions: `json_remove`, `find`, `replace`, `find_reg`, `replace_reg`.
- Added computed expressions: `get_queue()`, `get_last_prints()`.
- Added server commands: `@foreach`, `@endforeach`.
- Switch to disable manual moves when the printer is not homed.
- Direct login with `?apikey=user-api-key` if no session is active.
- Translated wizards.
- Custom blocking command list to prevent timeouts on unknown slow commands.

### Improved

- Klipper time prediction improved. There are special Klipper settings in the printer
  configuration, so please check them again.
- Linux GPIO solution drastically improved.
- Info is recomputed before a print starts, so computed expressions using `job...` are always
  correct during a print.
- Home Assistant discovery gets default precisions for all sensors.
- History PDFs now have the same name as on disk when saved.

### Fixed

- Deleting G-code replacements.
- Change filament dialog in the touch screen not saving distances.
- X-axis orientation for belt printers in 3D views.
- Print time prediction when "Run before job" contained temperature commands.
- Long report PDF with webcam image included.
- Security issues fixed.
- Many other small fixes and improvements.
