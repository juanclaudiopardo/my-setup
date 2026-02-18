# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

Personal documentation repo for Claude Code configuration. Contains installation references for MCP servers and skills — no application code, build system, or tests.

Language: Spanish (all documentation is written in Spanish).

## Structure

- `mcp/README.md` — MCP server installation commands (Playwright, shadcn/ui, Figma, Next.js DevTools, TanStack, Nx)
- `skills/README.md` — Skills CLI usage and installed skills (Vercel React Best Practices, Next.js Best Practices, Next.js Upgrade, Vercel Composition Patterns, Web Design Guidelines, SEO Audit, Nx Workspace Skills), plus AGENTS.md guidance

## Key References

- Skills CLI: `npx skills@latest` (add, list, find, check, update, remove, init)
- AGENTS.md generation for Next.js projects: `npx @next/codemod@canary agents-md`
- Nx AI agents setup (skills + MCP + CLAUDE.md): `npx nx configure-ai-agents`
