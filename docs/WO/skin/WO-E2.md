Title: Refactor `Includes_Hubs.xml` for Centralized Widget List
Objective: To introduce a centralized horizontal `list` control (mimicking AH2's ID 301) for widgets within `Includes_Hubs.xml`, aiming for a consistent hub grouping structure.
Scope: `skin.arctic.fuse.2.frankenpi/1080i/Includes_Hubs.xml`.
Files explicitly forbidden to modify: Any individual hub XML files (e.g., `Custom_1101_Hub_Movies.xml`), any JSON files.
Implementation notes:
1.  Open `skin.arctic.fuse.2.frankenpi/1080i/Includes_Hubs.xml`.
2.  Analyze AH2's `https://github.com/jurialmunkey/skin.arctic.horizon.2/blob/master/1080i/Includes_Hubs.xml` specifically focusing on the `Hub_Grouplist` (ID 301) definition and how it handles content (`control type="list"`).
3.  Refactor existing widget group definitions in AF2's `Includes_Hubs.xml` to integrate a similar centralized `list` control for widgets. This involves:
    *   Creating a new `include` or modifying an existing one to define a central `control type="list"` with a fixed ID (e.g., `301` for consistency with AH2) to house widgets.
    *   Adjusting existing widget references to point to this new centralized list.
    *   Ensure proper `onup`/`ondown` navigation is set for this list control.
Testing checklist:
- Launch Kodi and navigate to various hubs (e.g., Movies, TV Shows).
- Verify that widgets within these hubs are displayed consistently through the new centralized list control.
- Test horizontal and vertical navigation within the widget areas.
- Ensure no unexpected visual changes or navigation issues arise in other parts of the skin.
Commit message format: REFACTOR: Centralize widget list in Includes_Hubs.xml