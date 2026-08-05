# SourceDoc Pro
**Version 2.00 — August 2026**
*MWC Freeware — Michael W. Cetera*

## Overview

SourceDoc Pro is a free Windows utility that prints VB6 source code
with syntax highlighting, loop bracket connectors, form image rendering,
and procedure dependency reports for developer documentation and code
review.

SourceDoc Pro now includes several Developer Aids that can modify the
project code, with more tools to come in future releases (user
suggestions welcomed).

## What's New

See the [release notes](https://github.com/MwC-GitHub/SourceDoc-Pro/releases)
for version history.

## Version History

- **2.00:** added Form Image rendering showing all controls with their
  positions and names on the form; separate images showing the layering of
  overlapping controls; a separate page showing a complete menu tree for the
  form; several developer tools with more to come (suggestions welcomed);
  automatic removal of a few legacy suppressed-message listings — only those
  whose buttons or wording changed enough that a stored response no longer
  means what it did when it was saved — which may result in the display of a
  message previously thought suppressed; a significant number of warning
  messages made suppressible; User Manual revised to reflect code changes;
  corrected spelling errors in program messages and printed output.
  Improvements: opening a project is substantially faster, with a
  "Phase 3 of 3" progress count shown while the procedure index is
  completed; warning messages are now raised only for the setting that was
  actually changed, so editing one option no longer produces warnings about
  unrelated settings; the recommended margin adjustment now offers "Yes,
  But Only For This Session" as a direct choice instead of asking a second
  question; with Mimic IDE View set to No, User Options no longer asks
  about the font, the typical longest code line or the margins; the File
  menu and the Send To Target button always name the same output device,
  and that is the device output will actually go to; installing over an
  earlier version no longer asks you to accept the license agreement again;
  the notice shown before a split PDF run now explains that the printer
  driver's file name window will open and close in a flash for each
  temporary part and is filled in automatically; if a split print run is
  interrupted while that file name window is open, the notice now also
  explains that you can pick the run back up by pasting the next temporary
  file name, which is already on the clipboard; text boxes on the User
  Options screen now select their contents when they receive the focus.
  Major bug fixes: corrected missing print lines on some print runs;
  increased the read buffer to accommodate retrieval of large volume
  persistent data; corrected bolding for wrapped lines where only the last
  child was printed bold; corrected a User Options failure in which Save and
  Exit could do nothing at all, with no warning and no message, leaving the
  screen appearing to be frozen; a margin value that fails validation now
  always says which margin is at fault and why; a recommended margin
  adjustment accepted for the current session only is now correctly left out
  of the saved settings, and is shown in blue on the Options screen while it
  is in effect; the User Options screen now names the output device that will
  actually be used rather than the saved device, shown in blue when it applies
  to SourceDoc Pro's output only, and the File menu and Send To Target button
  name that same device; the Send To Target button caption no longer keeps naming the
  previous device after an output device is chosen from the File menu; a
  page size, page orientation or GDI Spool Size change made on its own
  could not be saved, because Save and Exit stayed disabled; leaving User
  Options with Exit rather than Save no longer resets the paper size to
  Letter and the orientation to Portrait; a left or right margin typed by
  hand now takes effect on the next print run rather than being ignored
  until the program was restarted; the Bottom margin box is no longer
  disabled, which previously happened whenever Duplex printing was set to
  No — the normal setting; a large print run to a PDF file no longer stops
  part way through with a Subscript out of range error, which could end the
  job early and leave the temporary files written up to that point on disk
  uncombined with the remaining selected procedures unprinted; with property
  aggregation selected, the individual Get/Let/Set Property procedures were
  left out of both the Procedures List and the Table of Contents, so a
  file's property procedures were missing from the printed documentation
  entirely — they are now always listed, and the aggregate is offered in
  addition to them rather than in place of them
- **1.10:** added option to change theme color; trapped unable to find
  default printer error, added trap to split file print of procedures that
  are too large for spooling resources, fixed bug when wrapped line has no
  convenient break causing infinite loop, added new default colors; other
  bug fixes, minor cosmetic changes
- **1.00:** original release

## Features

- Syntax highlighting for keywords, comments, strings, and operators
- Visual loop bracket connectors showing nested block structure
- Form Image rendering showing every control in position with its name
- Separate images showing how overlapping controls are layered
- Complete menu tree page for each form
- Procedure dependency reports showing Called By and Calls relationships
- Printable Table of Contents listing all project files and procedures
- Built-in developer tools
- Output to printer, PDF, or text file
- Flexible options including paper size, orientation, duplex printing,
  margin control, font selection, and aggregate procedure grouping
- Optional IDE-style code view mirroring the VB6 IDE appearance
- Viewable/Printable User Manual included
- Simple installer handles all setup automatically

## Requirements

- Windows 7 or later (32-bit or 64-bit) including arm64 processor
- VB6 runtime (included with Windows 7 and later — no separate download)

## Download

[Download SourceDocProSetup_v200.exe](https://github.com/MwC-GitHub/SourceDoc-Pro/releases/download/V2.00/SourceDocProSetup_v200.exe)

## Support

Email: VB3373@gmail.com

## Donate

If you find SourceDoc Pro useful, a voluntary donation to support continued
development is appreciated:
[Buy Me a Coffee](https://buymeacoffee.com/mwc_freeware_support)

## License

Freeware — free for personal and professional use.
Copyright 2025-2026 Michael W. Cetera. All Rights Reserved.

SourceDoc Pro bundles qpdf (Apache License 2.0) to combine split PDF
output. The qpdf license is installed under `qpdf Files\`.
