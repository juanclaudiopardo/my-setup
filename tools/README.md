# Tools

Herramientas CLI independientes (no son skills instaladas via `npx skills add`).

---

## React Doctor

**Descripción:** Escanea un proyecto React y sugiere mejoras de performance, configuración y buenas prácticas.

**Uso:**

```bash
npx -y react-doctor@latest
```

---

## rnsec

**Descripción:** Static analysis security scanner para apps React Native y Expo. Detecta vulnerabilidades sin configuración y genera reportes JSON/HTML aptos para CI/CD.

**Docs:** https://www.rnsec.dev/docs

**Instalación (global):**

```bash
npm install -g rnsec
```

**Verificar instalación:**

```bash
rnsec --version
```

**Uso (desde la raíz del proyecto RN/Expo):**

```bash
rnsec scan
```

**Requisitos:** Node.js 14+ y un proyecto React Native o Expo existente.
