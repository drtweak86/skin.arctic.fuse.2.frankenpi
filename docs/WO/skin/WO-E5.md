Title: Integrate AF3 Layout Refinements into Key Hubs
Objective: To apply specific, impactful layout refinements from Arctic Fuse 3 to the Movies and TV Shows hubs.
Scope: `skin.arctic.fuse.2.frankenpi/1080i/Custom_1101_Hub_Movies.xml`, `skin.arctic.fuse.2.frankenpi/1080i/Custom_1102_Hub_TVShows.xml`.
Files explicitly forbidden to modify: `skin.arctic.fuse.2.frankenpi/1080i/Includes_Hubs.xml`, any JSON files.
Implementation notes:
1.  Review Arctic Fuse 3 (`https://github.com/jurialmunkey/skin.arctic.fuse.3`) for general layout improvements (e.g., optimized spacing around widgets, improved text readability, or modern component arrangements specific to hub content).
2.  Select one or two *specific* layout refinements (e.g., adjusting the `margin`, `padding`, `itemgap`, or `font` size of a particular control within widgets) that can be directly applied to `Custom_1101_Hub_Movies.xml` and `Custom_1102_Hub_TVShows.xml`.
3.  Focus on refinements that enhance visual appeal and user experience without requiring a global structural change.
Testing checklist:
- Launch Kodi and navigate to the Movies Hub (Window 1101) and TV Shows Hub (Window 1102).
- Visually inspect the layout for the implemented refinements.
- Compare the appearance to the Arctic Fuse 3 reference (if possible) to ensure the changes are correctly applied.
- Ensure the refinements do not negatively impact readability or navigation.
Commit message format: REFACTOR: Integrate AF3 layout refinements in Movies and TV Hubs