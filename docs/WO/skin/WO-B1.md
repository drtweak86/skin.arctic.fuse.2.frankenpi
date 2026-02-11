Title: Add Search Menu Item to Home
Objective: To add a dedicated "Search" menu item to the main home menu.
Scope: `skin.arctic.fuse.2.frankenpi/shortcuts/skinvariables-shortcut-homemenu.json` (or `shortcuts/prebuilt/tmdb-basic/skinvariables-shortcut-homemenu.json` if that's the active source). Larry must determine the correct active source file.
Files explicitly forbidden to modify: `1080i/Custom_1185_Search.xml`, any other JSON files, any XML files.
Implementation notes:
1.  Open the active home menu JSON definition file.
2.  Add a new JSON object to the main array for "Search".
3.  Set its `"label"` to `"Search"`.
4.  Set its `"path"` to `"ActivateWindow(1185)"`.
5.  Set its `"icon"` to `"special://skin/extras/icons/search.png"`.
6.  Ensure unique `sidemenu_guid` and `guid` values are assigned (e.g., "guid-search-home", "guid-search-item").
Testing checklist:
- Launch Kodi with the modified skin.
- Verify that a "Search" menu item is present on the main home screen.
- Select the "Search" menu item and confirm that Window 1185 (the search screen) opens correctly.
- Ensure existing menu items function as expected.
Commit message format: FEAT: Add Search menu item to home