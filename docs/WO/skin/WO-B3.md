Title: Optimize Search Results Layout (Window 1185)
Objective: To improve the layout and visual presentation of search results within the search window (1185) for a "Netflix-style" experience.
Scope: `skin.arctic.fuse.2.frankenpi/1080i/Custom_1185_Search.xml`.
Files explicitly forbidden to modify: Any JSON files, any other XML files.
Implementation notes:
1.  Open `skin.arctic.fuse.2.frankenpi/1080i/Custom_1185_Search.xml`.
2.  Locate the control responsible for displaying search results (e.g., a `list` or `panel` control).
3.  Adjust layout properties (`itemlayout`, `focusedlayout`, `viewtype`) to present results in a visually appealing "Netflix-style" format (e.g., prominent artwork, clear text, possibly a grid or cinematic view).
4.  Ensure consistency with existing skin view styles where appropriate.
Testing checklist:
- Launch Kodi and perform a search in Window 1185.
- Verify that search results are returned and displayed in an optimized, "Netflix-style" layout.
- Confirm that result items are easy to browse and select.
- Check that selecting a result leads to the expected content information.
Commit message format: REFACTOR: Optimize Search results layout in Window 1185