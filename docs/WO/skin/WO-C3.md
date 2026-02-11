Title: Add "In-Progress Movies" Widget Item
Objective: To add a widget displaying movies currently in progress to the "Videos" section.
Scope: `skin.arctic.fuse.2.frankenpi/shortcuts/skinvariables-shortcut-homemenu.json` (or `shortcuts/prebuilt/tmdb-basic/skinvariables-shortcut-homemenu.json`). Larry must determine the correct active source file.
Files explicitly forbidden to modify: Any `.xsp` or `.xml` playlist files, any XML files.
Implementation notes:
1.  Open the active home menu JSON definition file.
2.  Locate the "Videos" menu item and its `widgets` array.
3.  Add a new JSON object for the "In-Progress Movies" widget.
4.  Set its `"label"` to `"In-Progress Movies"`.
5.  Set its `"path"` to `"library://video/movies/inprogressmovies.xml"` (or a new smart playlist file like `special://skin/extras/playlists/InProgressMovies.xsp`).
6.  Set its `"icon"` to `"special://skin/extras/icons/timer.png"`.
7.  Ensure a suitable `widget_style` (e.g., "Landscape").
8.  This widget should also link directly to the "Movies Hub" (Window 1101) upon selection. This might require additional Kodi path formatting.
Testing checklist:
- Launch Kodi and navigate to the home screen.
- Verify that an "In-Progress Movies" widget appears under the "Videos" section.
- Play a movie partially, then return to the home screen and confirm it appears in this widget.
- Select an item from the widget and confirm it resumes playback or navigates to the Movies Hub.
Commit message format: FEAT: Add "In-Progress Movies" widget item