# Regcheq Design System — AI Context File

> Este archivo es la referencia principal para generar cualquier interfaz, presentación o componente visual de Regcheq. Léelo completo antes de producir cualquier output.

---

## Sobre Regcheq

Regcheq es una plataforma B2B de compliance, prevención de lavado de activos (AML) y KYC para empresas en Latinoamérica. El producto es sofisticado, de confianza y tecnológico. El tono visual es: **profesional, moderno, claro y confiable** — con toques de innovación (IA, automatización).

---

## Stack técnico preferido

- **Framework:** Next.js (App Router)
- **Styling:** CSS variables nativas o Tailwind CSS
- **Fuentes:** Google Fonts (Poppins + Inter + Outfit)
- **Íconos:** Lucide React o SVG inline

---

## Colores

### Brand
| Token | Hex | Uso |
|-------|-----|-----|
| `--color-primary` | `#0064e0` | Botones CTA, links, accents principales |
| `--color-navy` | `#040045` | Fondos oscuros, hero, headings sobre dark |

### UI
| Token | Hex | Uso |
|-------|-----|-----|
| `--color-text` | `#3e4867` | Texto de párrafo |
| `--color-text-light` | `#5a6688` | Texto secundario, captions |
| `--color-bg` | `#ffffff` | Fondo base |
| `--color-bg-soft` | `#f4f8ff` | Fondo de página, secciones alternas |
| `--color-bg-bento` | `#f7fbff` | Fondo de cards bento |
| `--color-border` | `#e6eef8` | Bordes de cards, divisores |

### Accent
| Token | Hex | Uso |
|-------|-----|-----|
| `--color-cyan-mid` | `#00b5d4` | Hover de botones, orbs decorativos |
| `--color-blue-mid` | `#24bdff` | Gradientes, highlights |
| `--color-green` | `#65db8d` | Éxito, badges positivos |
| `--color-purple` | `#781ff4` | Features de IA, elementos diferenciadores |

### Semántico
| Token | Hex | Uso |
|-------|-----|-----|
| `--color-warning` | `#ef8a42` | Alertas, warnings |
| `--color-error` | `#e83a3a` | Errores, riesgos |

---

## Tipografía

| Fuente | Uso | Pesos usados |
|--------|-----|-------------|
| **Poppins** | Headings de sección, títulos de cards | 600, 700, 800 |
| **Inter** | Body text, UI, párrafos, labels | 400, 500, 600 |
| **Outfit** | Heroes de marketing, displays grandes | 600, 700, 800 |

### Escala de tamaños clave
- Hero H1: `4.5rem` / `clamp(2.5rem, 4.8vw, 4.8rem)` — weight 800, letter-spacing `-0.04em`
- Section H2: `2.8rem` — weight 800, letter-spacing `-0.03em`
- Card H3: `1.3rem–1.5rem` — weight 600
- Body: `1rem–1.18rem` — line-height `1.6`

---

## Gradientes

```css
/* Hero/banner oscuro */
background: linear-gradient(135deg, #040045 0%, #041668 45%, #0064e0 100%);

/* Botón primario */
background: linear-gradient(135deg, #00a8ff 0%, #0064e0 100%);

/* Texto destacado */
background: linear-gradient(135deg, #0064e0 0%, #24bdff 100%);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
```

---

## Componentes clave

### Botón Primario
```css
background: linear-gradient(135deg, #00a8ff 0%, #0064e0 100%);
color: #fff;
padding: 0 24px;
min-height: 54px;
border-radius: 14px;
font-weight: 700;
box-shadow: 0 16px 36px rgba(0, 100, 224, 0.35);
/* hover: translateY(-2px) */
```

### Card estándar
```css
background: #ffffff;
border: 1px solid #e6eef8;
border-radius: 20px;
padding: 40px;
/* hover: translateY(-8px), border-color rgba(0,100,224,0.2) */
```

### Hero oscuro
```css
background: linear-gradient(135deg, #040045 0%, #041668 45%, #0064e0 100%);
/* Overlay de grid: rgba(255,255,255,0.03) 40px */
/* Orbs decorativos con blur y animación */
```

### Badge / Eyebrow (fondo claro)
```css
background: rgba(255,255,255,0.82);
border: 1px solid rgba(0,100,224,0.12);
color: #0064e0;
border-radius: 9999px;
padding: 10px 16px;
font-weight: 700;
```

---

## Reglas de diseño

1. **Sobre fondos claros:** texto siempre en `--color-navy` o `--color-text`. Nunca negro puro `#000`.
2. **Sobre fondos oscuros (navy):** texto `#ffffff`, subtexto `#c7eeff` o `rgba(233,244,255,0.9)`.
3. **Border-radius:** preferir valores grandes (14px–34px). El sistema es suave y redondeado.
4. **Sombras:** siempre con color (navy o primary), nunca `box-shadow: 0 0 0 rgba(0,0,0,x)`.
5. **Spacing:** usar múltiplos de 4px. Padding de secciones mínimo 80px vertical.
6. **Efectos:** glassmorphism sutil permitido sobre dark (`rgba(255,255,255,0.08)` + blur). Evitar sobre light.
7. **Animaciones:** sutiles. Solo `translateY(-2px a -8px)` en hover. Sin efectos de entrada agresivos.
8. **Colores de acento (purple, green, cyan):** solo para features específicos, badges o íconos. No como color principal.

---

## Cómo usar este archivo

Al iniciar cualquier tarea de diseño o desarrollo:

```
Lee el design system en:
https://raw.githubusercontent.com/[usuario]/regcheq-design-system/main/CONTEXT.md

Luego: [describe lo que necesitas]
```

Para importar las variables CSS en cualquier proyecto:
```css
@import url('https://raw.githubusercontent.com/[usuario]/regcheq-design-system/main/tokens/variables.css');
```

O copia el contenido de `tokens/variables.css` directamente en tu proyecto.
