# AGENTS

Project notes for agents working in this repo.

- Runtime/build: Bun.
- Language: TypeScript with strict settings.
- Sources live in `/sources`; entry point is `sources/main.ts`.
- Subcommands live in `/sources/commands/<name>`.
- Shared helpers live in `/sources/utils`.
- Path alias: `@/` maps to `/sources`.
- Build: `bun run build` -> `dist/bee` (binary name `bee`).
- Package name: `bee-cli`.
- Typecheck: `bun run typecheck`.
- Commit after each successful step using Angular-style (conventional) commit messages.
- Before any commit: run `bun install`, `bun run typecheck`, and `bun run build`.

## Backup and archive policy

- Do not create additional backup or archive copies of content that can be recovered from Git history.
- Any necessary backup or archive copies must be placed under the owning project's `tmp/` directory.
- The project's `tmp/` directory and everything inside it must remain untracked and ignored by Git. Verify this before writing copies there; add `/tmp/` to the project's `.gitignore` if necessary. Never force-add these copies.
- These rules take precedence over conflicting backup-location or duplicate-copy instructions in this file.
