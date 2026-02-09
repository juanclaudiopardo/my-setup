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

---

## Skills Instaladas

### Vercel React Best Practices

**Descripción:** Proporciona mejores prácticas de React recomendadas por Vercel para desarrollo con Next.js y React moderno.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-react-best-practices
```

---

### Next.js Best Practices

**Descripción:** Mejores prácticas específicas para desarrollo con Next.js, incluyendo App Router, Server Components, y optimizaciones.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/next-skills --skill next-best-practices
```

---

### Next.js Upgrade

**Descripción:** Ayuda a migrar y actualizar proyectos Next.js a versiones más recientes con guías de breaking changes.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/next-skills --skill next-upgrade
```

---

### Vercel Composition Patterns

**Descripción:** Patrones de composición de componentes recomendados por Vercel para arquitectura escalable y reutilizable.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-composition-patterns
```

---

### Web Design Guidelines

**Descripción:** Guías y mejores prácticas de diseño web para interfaces modernas, accesibles y con buena UX.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill web-design-guidelines
```

---

### Vercel React Native Skills

**Descripción:** Mejores prácticas y patrones para desarrollo con React Native recomendados por Vercel.

**Instalación:**

```bash
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-react-native-skills
```

---

### Vitest

**Descripción:** Mejores prácticas y patrones para testing con Vitest, el framework de testing rápido y moderno compatible con Vite.

**Instalación:**

```bash
npx skills add https://github.com/antfu/skills --skill vitest
```

---

### SEO Audit

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

## AGENTS.md (Recomendado por Vercel)

Alternativa a skills. Un archivo markdown en la raíz del proyecto que da contexto persistente al agente en cada interacción, sin depender de que se invoque una skill.

En evals de Vercel, AGENTS.md logró **100% de éxito** vs 53% de skills por defecto.

**Generar AGENTS.md para un proyecto Next.js:**

```bash
npx @next/codemod@canary agents-md
```

Detecta tu versión de Next.js y genera el archivo con la documentación comprimida.

> Fuente: https://vercel.com/blog/agents-md-outperforms-skills-in-our-agent-evals
