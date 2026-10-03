# SourceDoc Pro
**Version 2.10 — October 2026**
*MWC Freeware — Michael W. Cetera*

## Overview

SourceDoc Pro is a free Windows utility that prints VB6 source code
with syntax highlighting, loop bracket connectors, form image rendering,
and procedure dependency reports for developer documentation and code
review.

Version 2.10 greatly expands the Developer Aids menu, which edits the
project's source in place: file and procedure headers, indenting,
long-line wrapping, line numbering, spell checking, project hygiene
checks and project statistics, all with automatic backups and restore
(user suggestions for more aids are welcomed).

## What's New

See the [release notes](https://github.com/MwC-GitHub/SourceDoc-Pro/releases)
for version history.

## Version History

- **2.10:** expanded the Developer Aids menu: Insert File Header and Insert
  Procedure Header from editable templates, including aids to relocate
  headers and to convert legacy headers; Indent Code Lines; Wrap Too Long
  Lines; Shrink Multiple Blank Lines to 1; Move All Procedure Dimension
  Statements; Sort File Procedures; Spell Check of string literals and
  comments, with a custom dictionary and ignore list; Add and Remove Line
  Numbers; View Statistics; and a new Project Hygiene group that finds
  Variants defined by default, dead code, project files not included in
  the .vbp, missing Option Explicit statements, procedures and parameters
  without an explicit scope, and .vbp references that are not registered;
  View Aid Log shows what each aid changed.
  Improvements: a Developer Aid backs up each file it changes once each
  time a project is opened, as a whole file, and Restore Edited
  File/Procedure puts it back; backups older than 60 days are deleted when
  a project is opened — change or turn this off in File | User Options;
  after an aid has changed the project, further aids can still be used —
  reload the project with File | Open to restore selection, printing and
  View Statistics; settings and saved data now live in a new MWCFreeware
  folder, with each project's data and backups kept in its own folder, and
  an existing installation's data is moved there automatically on first
  run; the default header templates are installed for all projects and
  are never overwritten by a later installation; printing on one side puts 
  the binding margin on every page, and
  duplex printing turns the sheet on the edge that suits the binding edge;
  User Manual revised, with a new Developer Aids chapter.
  Bug fixes: a line-numbered procedure printed with loop brackets now
  starts the procedure signature, its header and its End line at the left
  margin, as in the IDE, rather than after the space reserved for line
  numbers, which made lines that fit in the IDE too long in the output;
  the program no longer starts a second copy of itself when one is already
  running; the color picker now opens on the color currently set
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
- Developer Aids that edit the source in place: file and procedure
  headers, indenting, long-line wrapping, blank-line shrinking, Dim
  relocation, procedure sorting, line numbering and spell checking
- Project Hygiene checks for Variants defined by default, dead code,
  files missing from the .vbp, missing Option Explicit, unspecified
  procedure and parameter scope, and unregistered references
- Project statistics
- Automatic backups of every file an aid changes, with restore
- Output to printer, PDF, or text file
- Flexible options including paper size, orientation, duplex printing,
  binding margin, margin control, font selection, and aggregate procedure
  grouping
- Optional IDE-style code view mirroring the VB6 IDE appearance
- Viewable/Printable User Manual included
- Simple installer handles all setup automatically

## Requirements

- Windows 7 or later (32-bit or 64-bit) including arm64 processor
- VB6 runtime (included with Windows 7 and later — no separate download)

## Download

[Download SourceDocProSetup_v210.exe](https://github.com/MwC-GitHub/SourceDoc-Pro/releases/download/V2.10/SourceDocProSetup_v210.exe)

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

SourceDoc Pro bundles Hunspell (MPL 1.1 / GPL 2 / LGPL 2.1) and the
en_US dictionary for its Spell Check aid, together with the MinGW runtime
libraries Hunspell needs. Their licenses are installed under
`Hunspell Files\Licenses\`.
