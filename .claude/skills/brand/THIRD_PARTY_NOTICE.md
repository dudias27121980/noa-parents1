# Third-party skill

This skill was imported from the open-source project **UI UX Pro Max**
(https://github.com/nextlevelbuilder/ui-ux-pro-max-skill), version 2.13.0,
by nextlevelbuilder, licensed under the MIT License (see `LICENSE` in the
upstream repository).

Dev-only `scripts/tests` were excluded from the import. Reviewed for
safety before installation (no network calls, no credential/env access
beyond expected config, no obfuscated code, no prompt injection); the one
`execFileSync` call in `sync-brand-to-tokens.cjs` only invokes the
sibling `generate-tokens.cjs` script in this same skill directory.
