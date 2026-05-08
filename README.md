# Regcheq Design System

Sistema de diseño de referencia para Regcheq. No es una librería publicada — es una fuente de verdad para desarrollo consistente con IA.

## Estructura

```
regcheq-design-system/
├── CONTEXT.md              ← 🤖 Archivo principal para pasar a la IA
├── tokens/
│   ├── colors.json         ← Paleta de colores completa
│   ├── typography.json     ← Fuentes, pesos, escala tipográfica
│   ├── spacing.json        ← Espaciado, radios, sombras, layout
│   └── variables.css       ← Variables CSS listas para copiar/importar
├── components/
│   └── patterns.md         ← Patrones de UI documentados
├── assets/
│   └── logos/              ← Logos en distintos formatos
└── docs/                   ← Documentación adicional
```

## Cómo usar con IA

### Opción 1 — URL directa (recomendada)
```
Lee el design system de Regcheq en:
https://raw.githubusercontent.com/[usuario]/regcheq-design-system/main/CONTEXT.md

Luego crea [lo que necesitas].
```

### Opción 2 — Pegar el contenido
Copia el contenido de `CONTEXT.md` directamente en el chat antes de describir tu tarea.

## Cómo usar en proyectos

Copia `tokens/variables.css` en tu proyecto y úsalo en tu CSS global:

```css
/* globals.css o app/layout.css en Next.js */
/* pega el contenido de tokens/variables.css aquí */
```

## Stack de referencia
- **Next.js** (App Router)
- **CSS Variables** nativas o Tailwind CSS
- **Google Fonts:** Poppins + Inter + Outfit
- **Íconos:** Lucide React
