## Layout
- `.local/` — Files and artifacts, kept out of Git tracking by default unless explicitly requested otherwise.
  - `dev/` — Local development root for arbitrary files and dirs. Preserve `.local/dev/.env`.
  - `notes/` — Documents used or produced during routine tasks, organized under `<MMDD>-<topic>/`.
    - `archived/<YYYY>/<MMDD>-<topic>/`
  - `tools/` — Reusable scripts and utilities.
- `.references/` — Add references to external repos as needed, using symbolic links (Windows: junctions). Clone new repos into `<projects-parent>/Projects/references/<repo-path>` (`<repo>` or `<namespace>/<repo>`) before linking them under `.references/<repo-path>`. The `<projects-parent>` defaults to `~` on Unix-like systems or D: on Windows, but may be adjusted based on disk capacity and storage persistence. Do not duplicate repos.
