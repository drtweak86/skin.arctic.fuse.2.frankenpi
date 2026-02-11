Title: Update Font.xml for Exo2 Default
Objective: To configure `Font.xml` to use Exo2 as the default font.
Scope: `skin.arctic.fuse.2.frankenpi/1080i/Font.xml`.
Files explicitly forbidden to modify: Any `.ttf` files, any JSON files.
Implementation notes:
1.  Open `skin.arctic.fuse.2.frankenpi/1080i/Font.xml`.
2.  Locate the `fontset` with `id="Default"` and change its `include` to `Font_Default_Exo2`.
3.  Add a new `fontset` definition for `Font_Default_Exo2`. This new definition should reference `Exo2-Bold.ttf` for `font_bold`, `Exo2-Regular.ttf` for `font_regular`, and `Exo2-Light.ttf` for `font_light`. Use existing `plot_linespacing` values from other fontsets (e.g., "Outfit (Experimental)") as a starting point.
Testing checklist:
- Launch Kodi with the modified skin.
- Verify that the default font displayed throughout the UI is now Exo2.
- Check various labels and text elements to ensure font rendering is correct and legible.
- Ensure no unexpected visual issues related to font sizing or spacing appear.
Commit message format: FEAT: Set Exo2 as default font in Font.xml