Title: Adjust Hub Navigation and Animations to Match AH2
Objective: To fine-tune navigation behavior and animations within and between hubs to mimic AH2's smooth transitions and focus behavior.
Scope: `skin.arctic.fuse.2.frankenpi/1080i/Includes_Hubs.xml`, `skin.arctic.fuse.2.frankenpi/1080i/Custom_1101_Hub_Movies.xml`, `skin.arctic.fuse.2.frankenpi/1080i/Custom_1102_Hub_TVShows.xml`, `skin.arctic.fuse.2.frankenpi/1080i/Custom_1108_Hub_Anime.xml`.
Files explicitly forbidden to modify: Any JSON files, any other XML files.
Implementation notes:
1.  Analyze AH2's `Includes_Hubs.xml` for `onup`, `ondown`, `onback`, `onfocus` properties within its `Hub_Grouplist` and other navigation controls. Also, study its `WindowOpen` and `WindowClose` animations.
2.  Modify the corresponding navigation properties and animation definitions in AF2 Frankenpi's `Includes_Hubs.xml` and the specified individual hub XMLs to achieve similar responsiveness and visual flow.
3.  Pay attention to `tween` and `easing` parameters in animations for a smoother feel.
Testing checklist:
- Launch Kodi and navigate between different hubs and within a single hub.
- Compare the navigation experience (smoothness, speed, focus transitions) to reference AH2 behavior (if possible).
- Ensure all directional navigation (up, down, left, right) works as expected without skipping or getting stuck.
- Verify that opening and closing hubs has a fluid animation.
Commit message format: REFACTOR: Adjust hub navigation and animations