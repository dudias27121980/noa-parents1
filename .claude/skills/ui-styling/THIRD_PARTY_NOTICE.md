# Third-party skill

Imported from **UI UX Pro Max** (https://github.com/nextlevelbuilder/ui-ux-pro-max-skill),
version 2.13.0, by nextlevelbuilder, MIT License. Includes `canvas-fonts/`
(SIL Open Font License font files, each with its own `-OFL.txt` license
text) and `LICENSE.txt` (Apache 2.0, covering the shadcn/ui-derived
portions), both carried over from upstream unchanged.

Reviewed for safety before installation: the only subprocess call
(`shadcn_add.py`) runs `npx shadcn@<version> add <components>` via
`subprocess.run` with an argument list (no `shell=True`), matching
the standard/official shadcn/ui CLI installation flow. No network
calls beyond that npx invocation itself, no credential access, no
destructive file ops, no prompt injection.
