Title: Create Anime Content Smart Playlists
Objective: To provide the content sources for the widgets defined in the Anime Hub.
Scope: `skin.arctic.fuse.2.frankenpi/extras/playlists/*.xsp` (new files).
Files explicitly forbidden to modify: Any JSON files, any XML files (except new `.xsp` files).
Implementation notes:
1.  Create several new `.xsp` (smart playlist) files within the `skin.arctic.fuse.2.frankenpi/extras/playlists/` directory. These playlists should correspond to the widgets defined in `skinvariables-1108menu-widgets`.
2.  Examples:
    *   `RecentlyAddedAnime.xsp`: Filters video library for recently added content marked as "anime" (or by genre/path).
    *   `TrendingAnime.xsp`: Might integrate with an add-on or specific filters for trending anime.
    *   `AnimeGenres.xsp`: Lists anime content categorized by genre.
3.  Populate each `.xsp` file with appropriate Kodi smart playlist XML rules.
Testing checklist:
- Launch Kodi, navigate to the home screen, and select the "Anime" menu item.
- Verify that the widgets in the Anime Hub now populate with actual anime content.
- Ensure the content in each widget is relevant to its label (e.g., "Recently Added Anime" shows recent anime).
- Test browsing within the widgets and selecting content.
Commit message format: FEAT: Create Anime smart playlists