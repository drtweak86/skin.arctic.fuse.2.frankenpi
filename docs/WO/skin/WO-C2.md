Title: Create "Because You Watched" Smart Playlist
Objective: To define the content source for the "Because You Watched" widget.
Scope: `skin.arctic.fuse.2.frankenpi/extras/playlists/BecauseYouWatched.xsp`.
Files explicitly forbidden to modify: Any JSON files, any XML files (especially `skinvariables-shortcut-homemenu.json`).
Implementation notes:
1.  Create a new file named `BecauseYouWatched.xsp` in the `skin.arctic.fuse.2.frankenpi/extras/playlists/` directory.
2.  Populate this `.xsp` file with Kodi smart playlist XML structure.
3.  The playlist should include rules to dynamically select content (movies/TV shows) that are related to recently watched items (e.g., same genre, same director, similar actors), providing a "Because You Watched" experience. This will likely involve using Kodi's `limit` and `order` by functions.
Testing checklist:
- Launch Kodi and navigate to the home screen.
- Verify that the "Because You Watched" widget, when selected, displays a curated list of content.
- Ensure the content list appears logical based on recently watched items (if applicable).
Commit message format: FEAT: Create BecauseYouWatched.xsp smart playlist