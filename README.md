# RBTray

RBTray is a small Windows program that runs in the background and allows almost any window to be minimized to the system tray by:

- Right-Clicking its minimize button
- Shift-Right-Clicking on its title bar
- Using the Windows-Alt-Down hotkey

Note that not all all of these methods will work for every window, so please use whichever one works for your needs.

RBTray is free, open source, and is distributed under the terms of the [GNU General Public Licence](http://www.gnu.org/copyleft/gpl.html).

## Download

- [64 bit binaries](x64)
- [32 bit binaries](x86)
- [Original RBTray](http://sourceforge.net/projects/rbtray/files/)

## Installing

Download either the 32-bit or 64-bit binaries (depending on your OS) to a folder,
for example "C:\Program Files\RBTray".  Double click RBTray.exe to start it.  If
you want it to automatically start after you reboot, create a shortcut to RBTray.exe
in your Start menu's Startup group.

## Using

To minimize a program to the system tray, you can use any of these methods:

- Right-click with the mouse on the program's minimize button.
- Hold the Shift key while Right-clicking on the program's title bar.
- Pressing Windows-Alt-Down on the keyboard (all at the same time).

This should create an icon for the window in the system tray. To restore the
program's window, single-click the program's icon in the tray. Alternatively,
you can Right-click on the tray icon which should bring up a popup menu, then
select Restore Window.

## Exiting

Right click on any tray icon created by RBTray and click Exit RBTray in the
popup menu, or run RBTray.exe with the --exit parameter.

## Change history

- 4.8 fork (2018-Jul-27) - Benbuck Nason
  - Don't minimize desktop/taskbar/etc.
  - Return correct value from WinMain.
  - Allow processing of quit message.
  - Clean up handling of WM_TASKBAR_CREATED.

- 4.7 fork (2018-Jul-21) - Benbuck Nason
  - Support minimizing with Win-Alt-Down hotkey.

- 4.6 fork (2017-Aug-29) - Benbuck Nason
  - Fix compatibility issue with some Windows 10 64 bit environments.

- 4.5 fork (2017-May-12) - Benbuck Nason
  - Add some error handling.
  - Fix bug in shift key check.
  - Update project files to VS2015.

- 4.4 fork (2015-Dec-05) - Benbuck Nason:
  - Support minimizing by shift-right-clicking on window title bar.

- 4.3 (2011-Oct-30):
  - Hide windows instead of minimizing and hiding.
  - Hide windows even if they're already in the tray.
  - Fix "Close Window" for Explorer windows.

- 4.2 (2011-Jun-24):
  - Improve ability to minimize certain programs.

- 4.1 (2010-May-08):
  - Unified mouse hook procedure improves reliability and fixes small minimize target with XP theming.
  - Fixed tooltip overflow for long window captions.

- 4.0 (2010-May-06):
  - Alternative mouse hook procedure for Windows Vista/7 Aero compatibility.
  - Fixed 64-bit compatibility and created 64-bit compiles.
  - Removed window menu additions (e.g. Minimize in tray, Always on top), hotkey, and keyboard indicator.
  - Dropped Windows 9x support.
  - Tray icon tooltip can display Unicode characters.
  - Removes tray icon automatically if a program shows itself or exits.
  - Fixed problem when minimizing Office 2007 windows.
  - Won't minimize MDI child windows.
  - Other small fixes and reorganized code.

## Other

For original forum, bug tracker, etc. see [RBTray SourceForge project page](http://sourceforge.net/projects/rbtray/).

Copyright &copy; 1998-2011 Nikolay Redko, J.D. Purcell

Copyright &copy; 2015 Benbuck Nason
