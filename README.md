# POWCEQ 3D Oven Configurator — Astro starter

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Astro (usually http://localhost:4321).

## Integrate into an existing Astro website

1. Install Three.js: `npm install three`
2. Copy `src/components/OvenConfigurator.astro` into your project's components directory.
3. Import and render the component in any Astro page:

```astro
---
import OvenConfigurator from '../components/OvenConfigurator.astro';
---
<OvenConfigurator />
```

## Current scope

- Parametric simplified 3D batch curing oven, adjustable internal width/depth/height.
- Orbit controls, door open/close, heating selection, finish selection.
- Quote email composer (no recipient configured; set your verified sales email in the `mailto:` link).
- JSON configuration export.
- Responsive design.

**Important:** Geometry is a conceptual preview. It is not a manufacturing drawing. The dimensions in the interface are internal nominal dimensions; outer geometry uses indicative wall allowances. Heating selections do not yet simulate thermal engineering, power or performance. Quote requests open the visitor's email app, not a server-side lead capture. For production, integrate your verified contact email or CRM/API endpoint, product-specific constraints, GDPR/privacy text, and CAD-derived GLB assets.
