# Plugins

Plugins instalados en Claude Code. Los plugins inyectan conocimiento contextual en tiempo real observando ediciones de archivos y comandos de terminal.

---

## Vercel Plugin

**Descripción:** Permite a Claude Code comprender el ecosistema Vercel en profundidad. Observa actividades en tiempo real (ediciones de archivos y comandos de terminal) e inyecta dinámicamente conocimiento sobre la plataforma. Incluye 47+ skills técnicas (Next.js, AI SDK, Turborepo, Vercel Functions, Routing Middleware), 3 agentes especializados (Arquitecto de IA, Experto en Deployment, Optimizador de Performance) y 5 comandos slash (`/bootstrap`, `/deploy`, `/env`, `/status`, `/marketplace`).

**Instalación:**

Dentro de claude

```bash
/plugin install vercel
```

> Fuente: https://vercel.com/changelog/introducing-vercel-plugin-for-coding-agents

---

## Expo Plugin

**Descripción:** Enseña a los agentes de IA cómo construir, desplegar y depurar apps con Expo y React Native de forma precisa y eficiente. Incluye 11 skills: construcción de UI nativa (`building-native-ui`), API routes (`expo-api-routes`), CI/CD workflows (`expo-cicd-workflows`), deployment (`expo-deployment`), dev client (`expo-dev-client`), Tailwind CSS (`expo-tailwind-setup`), Jetpack Compose (`expo-ui-jetpack-compose`), SwiftUI (`expo-ui-swift-ui`), data fetching (`native-data-fetching`), upgrade de SDK (`upgrading-expo`) y DOM components (`use-dom`).

**Instalación:**

Dentro de claude

```bash
/plugin marketplace add expo/skills
/plugin install expo
```

> Fuente: https://docs.expo.dev/eas/ai/skills/

---

## Security Guidance Plugin

**Descripción:** Hace que Claude revise sus propios cambios de código en busca de vulnerabilidades comunes mientras trabaja y las corrija en la misma sesión, antes de que el código llegue a un pull request. Funciona de forma automática (no hay nada que invocar). Revisa en tres niveles: 1) **en cada edición de archivo**, una coincidencia de patrones rápida sin llamada al modelo (detecta `eval`, `os.system`, `child_process.exec`, `pickle`, `dangerouslySetInnerHTML`, ediciones en `.github/workflows/`, etc.); 2) **al final de cada turno**, una revisión en segundo plano del diff de git que detecta bypass de autorización, IDOR, inyección, SSRF y criptografía débil; 3) **en cada commit o push que hace Claude**, una revisión agéntica más profunda que lee el código circundante para bajar los falsos positivos. Es el complemento en sesión de Code Review (que corre en los PR). Se puede extender con reglas propias vía `.claude/claude-security-guidance.md` (guía para el modelo) y `.claude/security-patterns.yaml` (patrones deterministas por edición). Usa Claude Opus 4.7 por defecto en las revisiones con modelo.

**Requisitos:** Claude Code CLI 2.1.144 o superior, Python 3.8+ en el `PATH`, y un repositorio git (las revisiones de fin de turno y de commit comparan contra el estado de git).

**Instalación:**

Dentro de claude

```bash
/plugin install security-guidance@claude-plugins-official
```

> Si el marketplace no aparece, primero correr `/plugin marketplace add anthropics/claude-plugins-official` y reintentar. Luego activarlo en la sesión actual con `/reload-plugins`. Conviene elegir scope de usuario para que cargue en todas las sesiones locales.

> Para sesiones en la nube o repos compartidos, declararlo en el `.claude/settings.json` del proyecto:
>
> ```json
> {
>   "enabledPlugins": {
>     "security-guidance@claude-plugins-official": true
>   }
> }
> ```

> Fuente: https://code.claude.com/docs/en/security-guidance
