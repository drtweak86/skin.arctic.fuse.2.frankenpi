Title: Acquire Exo2 Font Files
Objective: To obtain Exo2 font files (Regular, Bold, Light) for use in the skin.
Scope: External action; placing files into the `fonts/` directory.
Files explicitly forbidden to modify: Any XML files, any JSON files.
Implementation notes: Larry must externally acquire the three specified Exo2 font files. These files should be placed into the `skin.arctic.fuse.2.frankenpi/fonts/` directory. No existing files in this directory should be altered, only new files added.
Testing checklist:
- Verify `Exo2-Regular.ttf`, `Exo2-Bold.ttf`, and `Exo2-Light.ttf` are present in `skin.arctic.fuse.2.frankenpi/fonts/`.
- Ensure no other files in the `fonts/` directory were modified or removed.
Commit message format: FEAT: Acquire Exo2 font files