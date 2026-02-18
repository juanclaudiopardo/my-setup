# Skills

Skills y comandos personalizados para Claude Code.

## CLI de Skills

```bash
npx skills@latest
npx skills add <package>   # Instalar una skill
npx skills list            # Listar skills instaladas
npx skills find [query]    # Buscar skills
npx skills check           # Verificar actualizaciones
npx skills update          # Actualizar todas las skills
npx skills remove          # Eliminar skills instaladas
npx skills init [name]     # Crear una nueva skill
```

Para instalar una skill específica de un repo con múltiples skills:

```bash
npx skills add <owner/repo> --skill <skill-name>
```

Las skills funcionan con 18+ agentes de IA: Claude Code, GitHub Copilot, Cursor, Cline, y más.

---

## Skills Instaladas

### React y Next.js

Skills para construir aplicaciones React y Next.js performantes.

#### Vercel React Best Practices

**Descripción:** Guías de optimización de performance para React y Next.js con 40+ reglas en 8 categorías.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-react-best-practices
```

---

#### Vercel Composition Patterns

**Descripción:** Patrones de composición de React que escalan, evitando la proliferación de boolean props.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-composition-patterns
```

---

#### Vercel React Native Skills

**Descripción:** Mejores prácticas de React Native con 16 reglas cubriendo performance, arquitectura y patrones específicos por plataforma.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-react-native-skills
```

---

#### Next.js Best Practices

**Descripción:** Mejores prácticas de Next.js cubriendo convenciones de archivos, boundaries de RSC, patrones de datos, y más.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/next-skills --skill next-best-practices
```

---

#### Next.js Cache Components

**Descripción:** Cache Components y PPR de Next.js 16 para mezclar contenido estático, cacheado y dinámico.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/next-skills --skill next-cache-components
```

---

#### Next.js Upgrade

**Descripción:** Actualizar Next.js a la última versión usando guías de migración oficiales y codemods.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/next-skills --skill next-upgrade
```

---

#### CRA to Next.js Migration

**Descripción:** Guía completa para convertir proyectos Create React App a Next.js.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/migration-skills --skill cra-to-next-migration
```

---

#### Turborepo

**Descripción:** Guía del build system para monorepos JavaScript y TypeScript con cache de tareas y ejecución paralela.

**Instalación:**

```bash
npx skills add https://github.com/vercel/turborepo --skill turborepo
```

---

### AI SDK

Skills para construir aplicaciones con IA usando el Vercel AI SDK.

#### AI SDK

**Descripción:** Responde preguntas sobre el AI SDK y ayuda a construir features con IA incluyendo agentes, chatbots y sistemas RAG.

**Instalación:**

```bash
npx skills add https://github.com/vercel/ai --skill ai-sdk
```

---

#### AI Elements

**Descripción:** Librería de componentes basada en shadcn/ui para aplicaciones AI-native.

**Instalación:**

```bash
npx skills add https://github.com/vercel/ai-elements --skill ai-elements
```

---

#### Streamdown

**Descripción:** Renderer de React Markdown optimizado para streaming con seguridad integrada.

**Instalación:**

```bash
npx skills add https://github.com/vercel/streamdown --skill streamdown
```

---

### Diseño y UI

Skills para construir interfaces accesibles y performantes.

#### Web Design Guidelines

**Descripción:** Revisa código UI para cumplimiento de Web Interface Guidelines con 100+ reglas cubriendo accesibilidad, performance y UX.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill web-design-guidelines
```

---

#### Building Components

**Descripción:** Guía para construir componentes UI con accesibilidad, APIs componibles y theming.

**Instalación:**

```bash
npx skills add https://github.com/vercel/components.build --skill building-components
```

---

### Automatización de Browser

Skills para automatizar interacciones del navegador.

#### Agent Browser

**Descripción:** CLI de automatización del browser para agentes de IA incluyendo navegación, llenado de formularios, screenshots y extracción de datos.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-browser --skill agent-browser
```

---

### Deployment

Skills para deploy de aplicaciones en Vercel.

#### Vercel Deploy

**Descripción:** Deploy de aplicaciones y sitios web a Vercel al instante con auto-detección de framework para 40+ frameworks.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-deploy
```

---

#### Vercel CLI

**Descripción:** Deploy, gestión y desarrollo de proyectos en Vercel desde la línea de comandos.

**Instalación:**

```bash
npx skills add https://github.com/vercel/vercel --skill vercel-cli
```

---

#### Autoship

**Descripción:** Releases automatizados con clonado de repositorio, generación de changeset con IA, y publicación a npm.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/autoship --skill autoship
```

---

### Commerce

Skills para construir experiencias de comercio y pagos.

#### UCP (Universal Commerce Protocol)

**Descripción:** Protocolo Universal de Comercio para sesiones de checkout, pagos y operaciones de commerce.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agentic-commerce-skills --skill ucp
```

---

### Workflow

Skills para construir workflows durables y resilientes.

#### Workflow

**Descripción:** Funciones async durables y resilientes con lógica de retry y orquestación basada en steps.

**Instalación:**

```bash
npx skills add https://github.com/vercel/workflow --skill workflow
```

---

### JSON Render

Skills para el framework de UI generativa JSON Render.

#### JSON Render Core

**Descripción:** Paquete core para definición de schemas, creación de catálogos y streaming de specs.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/json-render --skill json-render-core
```

---

#### JSON Render React

**Descripción:** Renderer React que convierte specs JSON en árboles de componentes React.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/json-render --skill json-render-react
```

---

#### JSON Render React Native

**Descripción:** Renderer React Native para specs JSON con componentes estándar y data binding.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/json-render --skill json-render-react-native
```

---

#### JSON Render Remotion

**Descripción:** Renderer Remotion que convierte specs JSON de timeline en videos.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/json-render --skill json-render-remotion
```

---

#### Remotion Best Practices

**Descripción:** Mejores prácticas para creación de videos con Remotion en React con 30+ archivos de reglas.

**Instalación:**

```bash
npx skills add https://github.com/remotion-dev/skills --skill remotion-best-practices
```

---

### Utilidad

Skills de propósito general para workflows de agentes.

#### Find Skills

**Descripción:** Descubrir e instalar skills de agentes desde el directorio skills.sh.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/skills --skill find-skills
```

---

#### Before and After

**Descripción:** Herramienta de comparación de screenshots para capturar estados antes/después de páginas web.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/before-and-after --skill before-and-after
```

---

### Testing

Skills de testing de terceros.

#### Vitest

**Descripción:** Mejores prácticas y patrones para testing con Vitest, el framework de testing rápido y moderno compatible con Vite.

**Instalación:**

```bash
npx skills add https://github.com/antfu/skills --skill vitest
```

---

#### React Native Best Practices (Callstack)

**Descripción:** Mejores prácticas de React Native por Callstack cubriendo arquitectura, performance y patrones de desarrollo.

**Instalación:**

```bash
npx skills add https://github.com/callstackincubator/agent-skills --skill react-native-best-practices
```

---

#### React Native Testing Library

**Descripción:** Mejores prácticas y patrones para testing de componentes React Native usando React Native Testing Library de Callstack.

**Instalación:**

```bash
npx skills add https://github.com/callstack/react-native-testing-library --skill react-native-testing
```

---

### SEO

#### SEO Audit

**Descripción:** Permite realizar auditorías SEO de sitios web, analizar metadatos, estructura, y dar recomendaciones para mejorar el posicionamiento.

**Instalación:**

```bash
npx skills add https://github.com/coreyhaines31/marketingskills --skill seo-audit
```

#### Herramientas de Testing SEO

**Lighthouse** (integrado en Chrome)

Puntaje de 0 a 100 en: SEO, Performance y Accessibility.

```
1. Abrí tu sitio en Chrome
2. Click derecho → "Inspeccionar"
3. Pestaña "Lighthouse"
4. Click en "Analyze page load"
```

**Rich Results Test**

Valida el Schema.org (LocalBusinessSchema). Verifica si Google puede leer los datos estructurados.

```
1. Ir a https://search.google.com/test/rich-results
2. Poner la URL del sitio
3. Ver si el schema está bien o tiene errores
```

---

### Nx Workspace Skills

**Descripción:** Skills de workspace de Nx que enseñan al agente a usar generadores, CI, tareas, plugins y navegación del project graph. En lugar de exponer datos por MCP, Nx provee instrucciones específicas por dominio — la diferencia entre darle una llave inglesa a alguien y enseñarle a ser mecánico.

Skills incluidas:
- **Generator skills** — enseñan cuándo y cómo usar generadores de Nx
- **CI fix subagent** — análisis autónomo de errores y fixes
- **Project graph navigation** — exploración de dependencias del workspace

**Instalación:**

Se configura automáticamente junto con el MCP server y CLAUDE.md de Nx con un solo comando:

```bash
npx nx configure-ai-agents
```

> Requisito: necesitás tener Nx en tu proyecto. Si no lo tenés: `npx nx@latest init`

El comando detecta qué herramientas de IA tenés y genera las configuraciones correspondientes. Funciona para Claude Code, Cursor, Copilot, Gemini, Codex y OpenCode.

Ver también: [Nx MCP Server](../mcp/README.md#nx)

> Fuente: https://nx.dev/blog/why-we-deleted-most-of-our-mcp-tools

---

## AGENTS.md (Recomendado por Vercel)

Alternativa a skills. Un archivo markdown en la raíz del proyecto que da contexto persistente al agente en cada interacción, sin depender de que se invoque una skill.

En evals de Vercel, AGENTS.md logró **100% de éxito** vs 53% de skills por defecto.

**Generar AGENTS.md para un proyecto Next.js:**

```bash
npx @next/codemod@canary agents-md
```

Detecta tu versión de Next.js y genera el archivo con la documentación comprimida.

> Fuente: https://vercel.com/blog/agents-md-outperforms-skills-in-our-agent-evals
