---
description: Scaffold a new 3D design (folders + README + starter OpenSCAD file)
argument-hint: <design-name> [short description]
---

Create a new design named `$1` (convert to kebab-case) inside this project.

1. Create `models/$1/`, `exports/$1/`, `renders/$1/`, and `references/$1/`.
2. In `models/$1/`, write a `README.md` with sections: Purpose, Key dimensions (mm),
   Material / print settings, Status (start as "idea"). Use this description if given: $ARGUMENTS
3. In `models/$1/`, write a starter `$1.scad` with the main parameters declared at the top.
4. Follow the conventions in `CLAUDE.md`, then summarise what was created.
