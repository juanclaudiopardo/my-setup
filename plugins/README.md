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
