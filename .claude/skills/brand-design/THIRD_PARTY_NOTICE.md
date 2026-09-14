# Third-party skill

Imported from **UI UX Pro Max** (https://github.com/nextlevelbuilder/ui-ux-pro-max-skill),
version 2.13.0, by nextlevelbuilder, MIT License. Upstream folder name is
`design`; renamed to `brand-design` here because this project's session
already has a built-in `design` skill (Claude Design canvas) and the two
would otherwise collide on name.

Reviewed for safety before installation, with particular attention to
the logo/icon/CIP generation scripts, which make real outbound HTTPS
calls to Gemini, Atlas Cloud, or MuAPI:

- All three providers are opt-in and require the user's own API key
  (`GEMINI_API_KEY` / `GOOGLE_API_KEY`, `ATLASCLOUD_API_KEY`,
  `MUAPI_API_KEY`), read from environment variables or a local `.env`
  file — never hardcoded, never transmitted anywhere but the
  provider's own official API endpoint.
- Redirects from the image-generation APIs are validated by a
  `_SafeRedirectHandler` that rejects non-HTTPS, localhost/internal
  hostnames, and non-public IP addresses before following them —
  explicit SSRF hardening.
- No other network access, no credential harvesting, no destructive
  file ops, no prompt injection found.

Verdict: CAUTION-but-approved — the sensitive behavior (calling
external AI image APIs) is documented, opt-in, bounded to the user's
own key, and defensively coded. It stays inert unless the user
supplies an API key.
