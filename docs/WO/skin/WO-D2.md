Title: Add "Anime" Menu Item to Home
Objective: To add a dedicated "Anime" menu item to the main home menu.
Scope: `skin.arctic.fuse.2.frankenpi/shortcuts/skinvariables-shortcut-homemenu.json` (or `shortcuts/prebuilt/tmdb-basic/skinvariables-shortcut-homemenu.json`). Larry must determine the correct active source file.
Files explicitly forbidden to modify: `1080i/Custom_1108_Hub_Anime.xml`, any other JSON files, any XML files.
Implementation notes:
1.  Open the active home menu JSON definition file.
2.  Add a new JSON object to the main array for "Anime".
3.  Set its `"label"` to `"Anime"`.
4.  Set its `"path"` to `"ActivateWindow(1108)"`.
5.  Set its `"icon"` to `"special://skin/extras/icons/tv.png"` (or a more specific anime-related icon if available).
6.  Ensure unique `sidemenu_guid` and `guid` values are assigned (e.g., "guid-anime-home", "guid-anime-item").
Testing checklist:
- Launch Kodi with the modified skin.
- Verify that an "Anime" menu item is present on the main home screen.
- Select the "Anime" menu item and confirm that Window 1108 (which will become the Anime Hub) opens correctly.
- Ensure existing menu items function as expected.
Commit message format: FEAT: Add Anime menu item to home