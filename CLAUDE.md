# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

Personal documentation repo for Claude Code configuration. It records — as installation references — the MCP servers, skills, plugins, and standalone CLI tools the user keeps in their setup. There is no application code, build system, or tests; work here means editing Markdown.

Language: all documentation is written in Spanish. Match it when adding entries.

## Structure

Each top-level folder is one category, with a single `README.md` that lists its entries. `README.md` at the root links to all four.

- `mcp/README.md` — MCP servers (Playwright, shadcn/ui, Figma, Next.js DevTools, Maestro, Nx)
- `skills/README.md` — Skills CLI usage plus installed skills grouped by category (React/Next.js, AI SDK, Diseño/UI, Browser Automation, Deployment, Commerce, Workflow, JSON Render, Utilidad, Testing, SEO, Nx), and AGENTS.md guidance
- `plugins/README.md` — Installed plugins (Vercel, Expo, Security Guidance)
- `tools/README.md` — Standalone CLI tools that are *not* skills (React Doctor, rnsec)

## Which category an entry belongs to

This distinction is the main thing to get right when adding something new:

- **MCP server** — connects Claude to an external service/API; installed with `claude mcp add ...`
- **Skill** — installed via the Skills CLI (`npx skills add ...`) or shipped by a plugin
- **Plugin** — bundles skills/agents/commands/hooks; installed in-session with `/plugin install ...`
- **Tool** — a plain CLI run with `npx`/`npm`, no Claude integration

## Entry format convention

Every entry across all four READMEs follows the same shape, separated by `---`:

- `## <Name>`
- `**Descripción:**` — one paragraph in Spanish explaining what it does
- `**Instalación:**` (and/or `**Uso:**`) — a fenced command block
- optional `> Requisito:` / `> Fuente:` blockquotes for prerequisites and source links

Preserve this structure and the Spanish prose when adding or editing entries.

## Key References

- Skills CLI: `npx skills@latest` (add, list, find, check, update, remove, init)
- AGENTS.md generation for Next.js projects: `npx @next/codemod@canary agents-md`
- Nx AI agents setup (skills + MCP + CLAUDE.md): `npx nx configure-ai-agents`
