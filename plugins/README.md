# Plugins

Plugins instalados en Claude Code. Los plugins inyectan conocimiento contextual en tiempo real observando ediciones de archivos y comandos de terminal.

---

## Vercel Plugin

**Descripción:** Permite a Claude Code comprender el ecosistema Vercel en profundidad. Observa actividades en tiempo real (ediciones de archivos y comandos de terminal) e inyecta dinámicamente conocimiento sobre la plataforma. Incluye 47+ skills técnicas (Next.js, AI SDK, Turborepo, Vercel Functions, Routing Middleware), 3 agentes especializados (Arquitecto de IA, Experto en Deployment, Optimizador de Performance) y 5 comandos slash (`/bootstrap`, `/deploy`, `/env`, `/status`, `/marketplace`).

**Instalación:**

Dentro de claude

```bash
/claude plugin add vercel
```

> Fuente: https://vercel.com/changelog/introducing-vercel-plugin-for-coding-agents
