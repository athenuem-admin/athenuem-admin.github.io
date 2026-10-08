# 3D Designs

Workspace for 3D design projects: models, print/export files, renders, and reference material.

## Layout

| Folder        | Holds                                                        |
|---------------|--------------------------------------------------------------|
| `models/`     | Editable source files (`.blend`, `.scad`, `.f3d`, `.step`)   |
| `exports/`    | Output for printing/sharing (`.stl`, `.3mf`, `.obj`, `.glb`) |
| `renders/`    | Preview images (`.png`, `.jpg`)                              |
| `references/` | Sketches, measurements, inspiration images                   |

Each design gets its own subfolder inside each directory, named in `kebab-case`
(e.g. `models/phone-stand/`, `exports/phone-stand/`).

## Conventions

- Units are **millimetres** unless a file says otherwise.
- Prefer parametric sources (OpenSCAD, CadQuery) so dimensions are easy to tweak; keep key
  parameters at the top of the file with comments.
- Version exports by suffix: `phone-stand_v2.stl`. Never overwrite a previous version.
- Every design folder in `models/` gets a short `README.md`: purpose, key dimensions,
  material/print settings, and status (idea / in progress / done).
- Keep binary files under 25 MB; anything bigger should go in Git LFS or external storage.

## Notes for Claude

- This folder lives inside a GitHub Pages site (`athenuem-admin.github.io`). Anything committed
  here is publicly served, so don't commit private or licensed files.
- Don't edit files outside `3d-designs/` when working on a design.
- When generating geometry, write OpenSCAD (`.scad`) by default and describe how to export it.
