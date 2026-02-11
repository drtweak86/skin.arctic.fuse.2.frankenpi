Title: Create "In-Progress Movies" Smart Playlist (if needed)
Objective: To provide the content source for the "In-Progress Movies" widget.
Scope: `skin.arctic.fuse.2.frankenpi/extras/playlists/InProgressMovies.xsp` (or modify relevant XML if `library://video/movies/inprogressmovies.xml` is preferred). Larry must determine the best approach for defining in-progress movies content based on Kodi's capabilities.
Files explicitly forbidden to modify: Any JSON files, any other XML files.
Implementation notes:
1.  **Option 1 (Recommended)**: Create a new file named `InProgressMovies.xsp` in the `skin.arctic.fuse.2.frankenpi/extras/playlists/` directory. Populate it with Kodi smart playlist XML structure to filter for movies with "in progress" status.
2.  **Option 2 (Alternative)**: If `library://video/movies/inprogressmovies.xml` is intended to be a direct library node, ensure it's correctly configured in Kodi's video library settings.
Testing checklist:
- Launch Kodi.
- Partially play a movie.
- Navigate to the "In-Progress Movies" widget on the home screen.
- Verify that the partially played movie (and any others in progress) are correctly displayed in the widget.
Commit message format: FEAT: Create InProgressMovies smart playlist