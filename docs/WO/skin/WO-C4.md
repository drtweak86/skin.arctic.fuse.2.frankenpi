Title: Remove Trakt Widgets from Home (`homemenu.json`)
Objective: To remove all Trakt-related widgets from the generic home menu to comply with the "no watchlists on generic home" rule.
Scope: `skin.arctic.fuse.2.frankenpi/shortcuts/prebuilt/tmdb-basic/skinvariables-shortcut-homemenu.json`.
Files explicitly forbidden to modify: `shortcuts/prebuilt/tmdb-basic/skinvariables-shortcut-sidemenu.json`, any XML files.
Implementation notes:
1.  Open `skin.arctic.fuse.2.frankenpi/shortcuts/prebuilt/tmdb-basic/skinvariables-shortcut-homemenu.json`.
2.  Identify and remove all JSON objects from the `widgets` arrays that have `path` values referencing Trakt (e.g., `info=trakt_userlist`, `info=trakt_trending`). This includes entries like "Trending Movies", "Best Movies Last Decade", "Trending TV", "Highly Rated TV Shows", and "Shut Up, And Watch".
3.  Ensure proper JSON syntax is maintained after removal (e.g., correct comma placement).
Testing checklist:
- Launch Kodi and navigate to the home screen.
- Verify that no Trakt-related widgets or watchlists appear on the generic home screen.
- Ensure all other widgets and menu items function as expected.
Commit message format: FIX: Remove Trakt widgets from home menu