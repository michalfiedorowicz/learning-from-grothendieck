# Repository maintenance

Keep this repository portable, complete, and coherent when cloned onto another machine.

- Use relative internal links that resolve to committed files or headings within this repository.
- Do not make the collection depend on machine-specific paths, configuration, software installations, or files outside the repository.
- Keep absolute local paths, host-specific settings, and machine-specific working notes out of tracked files. Store such material in `.local/`, which is gitignored. If it must live elsewhere, add a targeted `.gitignore` rule before committing.
- Gitignore rules exclude files, not passages within files. Keep machine-specific material separate from the portable collection, and never require ignored material to understand or use it.
- Preserve valid internal links when moving or renaming files. Keep additions minimal; do not introduce unnecessary tooling or scaffolding.
