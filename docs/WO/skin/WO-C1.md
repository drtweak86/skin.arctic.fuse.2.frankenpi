Title: Add "Because You Watched" Widget Item
Objective: To introduce a "Because You Watched" widget to the "Videos" section of the home screen.
Scope: `skin.arctic.fuse.2.frankenpi/shortcuts/skinvariables-shortcut-homemenu.json` (or `shortcuts/prebuilt/tmdb-basic/skinvariables-shortcut-homemenu.json`). Larry must determine the correct active source file.
Files explicitly forbidden to modify: Any `.xsp` files, any XML files.
Implementation notes:
1.  Open the active home menu JSON definition file.
2.  Locate the "Videos" menu item and its `widgets` array.
3.  Add a new JSON object for the "Because You Watched" widget.
4.  Set its `"label"` to `"Because You Watched"`.
5.  Set its `"path"` to `"special://skin/extras/playlists/BecauseYouWatched.xsp"`.
6.  Set its `"icon"` to `"special://skin/extras/icons/eye.png"`.
7.  Ensure a suitable `widget_style` (e.g., "Landscape").
Testing checklist:
- Launch Kodi and navigate to the home screen.
- Verify that a "Because You Watched" widget appears under the "Videos" section.
- Ensure no other widgets or menu items were inadvertently affected.
Commit message format: FEAT: Add "Because You Watched" widget item