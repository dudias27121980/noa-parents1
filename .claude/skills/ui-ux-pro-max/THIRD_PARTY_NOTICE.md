# Third-party skill

This skill was imported from the open-source project **UI UX Pro Max**
(https://github.com/nextlevelbuilder/ui-ux-pro-max-skill), version 2.13.0,
by nextlevelbuilder, licensed under the MIT License (see `LICENSE` in the
upstream repository).

Only the `ui-ux-pro-max` skill itself was imported here (data, references,
and scripts under `scripts/tests` excluded). The upstream repository also
bundles several other skills (`banner-design`, `brand`, `design-system`,
`design`, `slides`, `ui-styling`) and a standalone CLI — none of those were
installed into this project.

The script invocation path in `SKILL.md` was adjusted from the upstream
plugin-relative `${CLAUDE_PLUGIN_ROOT}` form to a path relative to this
repository's root, since this skill is installed directly rather than
through a Claude Code plugin marketplace.
