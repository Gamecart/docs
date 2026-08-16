# Gamecart Docs

This repository contains Gamecart's public documentation.

This site is built with Mintlify and lives in `C:\Users\tanz\Documents\develop\gamecart\dev\repositories\docs`.

## Development

Run commands from this directory.

```bash
sfw.cmd npx mint dev
```

Use Socket Firewall for every package command in this workspace. If it blocks a package, do not bypass the warning.

## Content rules

- Public documentation is written in English by default.
- The internal `.docs/` vault remains in Portuguese-BR.
- Tutorials can explain workflows, but they must not invent backend behavior.
- API reference content must be generated from, or manually verified against, the current backend REST resources, DTOs, and OpenAPI output.
- Webhook documentation must be based on current backend callback contracts and vault notes.
- Never publish secrets, internal-only endpoints, callback tokens, or placeholder credentials.

## Structure

- `docs.json` controls navigation, branding, and global settings.
- `index.mdx` is the documentation home page.
- `quickstart.mdx` is the first setup path.
- `tutorials/` contains task-oriented guides.
- `api-reference/` is reserved for generated or verified API documentation.
- `webhooks/` is reserved for public webhook documentation.

## Publishing changes

Mintlify deployment runs outside this repository. This repository remains the source for published documentation.
