# MCP Servers

Servidores MCP (Model Context Protocol) instalados en Claude Code.

---

## Playwright

**Descripción:** Permite a Claude Code interactuar con navegadores web. Puede abrir páginas, hacer clicks, llenar formularios, tomar screenshots, extraer contenido y automatizar tareas de navegación.

**Instalación:**
```bash
claude mcp add playwright npx @playwright/mcp@latest
```

---

## shadcn/ui

**Descripción:** Permite a Claude Code agregar y gestionar componentes de shadcn/ui en proyectos React/Next.js. Puede instalar componentes, configurar temas y personalizar estilos.

**Instalación:**
```bash
npx shadcn@latest mcp init --client claude
```

---

## Figma

**Descripción:** Permite a Claude Code acceder a diseños de Figma. Puede leer archivos, extraer componentes, obtener estilos, colores y especificaciones de diseño para implementarlos en código.

**Instalación:**
```bash
claude mcp add --transport http figma https://mcp.figma.com/mcp
```

---

## Next.js DevTools

**Descripción:** Permite a Claude Code acceder a herramientas de desarrollo de Next.js. Puede inspeccionar rutas, componentes, configuración del proyecto y ayudar con debugging.

**Instalación:**
```bash
claude mcp add next-devtools npx next-devtools-mcp@latest
```

---

## TanStack

**Descripción:** Permite a Claude Code trabajar con el ecosistema TanStack (Query, Router, Table, Form). Puede ayudar a configurar, generar código y gestionar estas librerías en proyectos React.

**Instalación:**
```bash
claude mcp add tanstack -- npx @tanstack/cli mcp
```
