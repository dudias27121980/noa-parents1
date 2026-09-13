# Third-party skill

This skill was imported from the open-source project **UI UX Pro Max**
(https://github.com/nextlevelbuilder/ui-ux-pro-max-skill), version 2.13.0,
by nextlevelbuilder, licensed under the MIT License (see `LICENSE` in the
upstream repository).

Dev-only `scripts/tests` were excluded from the import. Reviewed for
safety before installation (no live network calls — `fetch-background.py`
only returns a curated, hardcoded list of Pexels image URLs and a Pexels
search-page URL string; it never performs an HTTP request itself. No
credential/env access beyond an optional `DESIGN_SYSTEM_PROJECT_ROOT`
override, no obfuscated code, no prompt injection).
