# Documentation project instructions

## Scope

- This repository contains the Tiny Exchange internal Mintlify site.
- Document the REST trading API, private and public WebSockets,
  authentication, canonical wire formats, recovery, and fee accounting.
- The exchange implementation lives in `tiny-xyz/tiny-exchange`; verify every
  behavioral claim against that repository before changing it here.
- Keep `api/external` aligned with the exchange repository's OpenAPI schemas.

## Style

- Use active voice and second person.
- Keep sentences concise and state present behavior without historical notes.
- Use sentence case for headings.
- Format paths, commands, field names, and wire values as code.
- State exact units and rounding rules for money and quantities.
- Do not invent behavior that is absent from the implementation or schemas.

## Structure and validation

- Pages are root-level MDX files with YAML frontmatter.
- Mintlify configuration lives in `docs.json`.
- OpenAPI schemas live under `api/external`.
- Run `npx --yes mintlify@latest validate` and
  `npx --yes mintlify@latest broken-links` before publishing.
