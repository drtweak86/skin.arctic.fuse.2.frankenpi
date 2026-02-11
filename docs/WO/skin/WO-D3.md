Title: Define Anime Hub Widgets (`skinvariables-1108menu-widgets`)
Objective: To configure the widgets and content categories for the new Anime Hub (Window 1108).
Scope: `skin.arctic.fuse.2.frankenpi/shortcuts/skinvariables-1108menu-widgets` (or create if missing). Larry must determine the correct location/filename for this widget definition based on skin conventions.
Files explicitly forbidden to modify: `1080i/Custom_1108_Hub_Anime.xml`, any actual playlist files (`.xsp`, `.xml`).
Implementation notes:
1.  Create a new JSON file (or modify an existing one if a generic `1108menu-widgets` exists) named `skinvariables-1108menu-widgets` in the `skin.arctic.fuse.2.frankenpi/shortcuts/` directory.
2.  Populate this file with JSON objects defining widgets relevant to anime content (e.g., "Recently Added Anime", "Trending Anime", "Anime by Genre", "Anime Watchlist").
3.  Each widget should have a `"label"`, `"path"` (referencing smart playlists or Kodi library nodes for anime), `"icon"`, and `"widget_style"`.
Testing checklist:
- Launch Kodi, navigate to the home screen, and select the "Anime" menu item.
- Verify that the Anime Hub (Window 1108) displays the newly defined widgets.
- Ensure that the widgets have appropriate labels and icons.
- Check that the widgets attempt to load content (even if the playlists are not yet created).
Commit message format: FEAT: Define Anime Hub widgets