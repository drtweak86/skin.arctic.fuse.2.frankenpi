Title: Implement Fullscreen Widget Artwork for Hubs
Objective: To integrate dynamic fullscreen background artwork display for hubs, similar to AH2's "Fullscreen Widget" concept.
Scope: `skin.arctic.fuse.2.frankenpi/1080i/Includes_Hubs.xml`, `skin.arctic.fuse.2.frankenpi/1080i/Includes_Images.xml`, `skin.arctic.fuse.2.frankenpi/1080i/Includes_Labels.xml`.
Files explicitly forbidden to modify: Any individual hub XML files, any JSON files.
Implementation notes:
1.  Open `skin.arctic.fuse.2.frankenpi/1080i/Includes_Hubs.xml`.
2.  Analyze AH2's `Hub_Grouplist` and "Fullscreen Widget" section for how it sets up `control type="image"` elements with `background="true"` and references to variables like `$VAR[Image_FullscreenWidget_Artwork]`.
3.  In AF2's `Includes_Hubs.xml`, introduce `control type="image"` elements configured to display dynamic background artwork behind the widgets.
4.  Modify `skin.arctic.fuse.2.frankenpi/1080i/Includes_Images.xml` to define the necessary `$VAR[Image_FullscreenWidget_Artwork]` (and potentially `_Artwork-1`, `_Artwork+1` for slide animations) variables to pull artwork from the currently focused widget item.
5.  Adjust animations (e.g., `fade`, `slide`) for the background artwork to create a smooth transition effect.
Testing checklist:
- Launch Kodi and navigate to various hubs.
- Focus on different widgets within a hub.
- Verify that a dynamic fullscreen background image (related to the focused widget item) is displayed.
- Observe the transitions and animations of the background artwork for smoothness.
Commit message format: FEAT: Implement fullscreen widget artwork for hubs