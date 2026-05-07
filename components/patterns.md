# Regcheq — Component Reference

Patrones de UI observados en los mockups del producto. Usar como referencia al generar nuevos componentes.

---

## Buttons

### Primary Button
- Background: `linear-gradient(135deg, #00a8ff 0%, #0064e0 100%)`
- Color: `#ffffff`
- Padding: `0 24px`, min-height: `54px`
- Border-radius: `14px`
- Font-weight: `700`
- Shadow: `0 16px 36px rgba(0, 100, 224, 0.35)`
- Hover: `translateY(-2px)`

### Secondary Button (sobre dark)
- Background: `rgba(255, 255, 255, 0.08)`
- Border: `1px solid rgba(255, 255, 255, 0.18)`
- Backdrop-filter: `blur(14px)`
- Color: `#ffffff`

### Secondary Button (sobre light)
- Background: `transparent`
- Border: `1px solid var(--color-border)`
- Color: `var(--color-text)`

---

## Cards

### Standard Card
- Background: `#ffffff`
- Border: `1px solid var(--color-border)`
- Border-radius: `20px`
- Padding: `40px`
- Hover: `translateY(-8px)`, `shadow-lg`, border-color `rgba(0, 100, 224, 0.2)`

### Bento Card
- Background: `var(--color-bg-bento)` → `#f7fbff`
- Misma estructura que Standard Card
- Variante wide: `grid-column: span 2`, flex row

### Dark/Navy Card (legal, CTAs)
- Background: `var(--color-navy)` → `#040045`
- Color texto: `#ffffff`
- Acento izquierdo: `6px solid linear-gradient(warning → error)`
- Shadow: `var(--shadow-navy)`

---

## Hero / Banner

### Hero Oscuro
- Background: `var(--gradient-hero)` con grid overlay `rgba(255,255,255,0.03)` 40px
- Orbs decorativos: `primary`, `purple (#781ff4)`, `cyan (#00b5d4)` con blur y animación
- Título: color `#ffffff`, font-size `4.5rem`, font-weight `800`, letter-spacing `-0.04em`
- Subtítulo: color `#c7eeff`

### Banner con glassmorphism
- Background del banner: `var(--gradient-hero)`
- Grid overlay sutil
- Orb glow en esquina: `rgba(69, 208, 255, 0.38)` con blur
- Surface cards: `rgba(255, 255, 255, 0.08)` con border `rgba(255,255,255,0.10)`

---

## Badges / Tags / Pills

### Eyebrow (sobre fondo claro)
- Background: `rgba(255, 255, 255, 0.82)`
- Border: `1px solid rgba(0, 100, 224, 0.12)`
- Color: `var(--color-primary)`
- Border-radius: `9999px`
- Padding: `10px 16px`
- Punto decorativo: `linear-gradient(135deg, cyan, blue)`

### Kicker (sobre fondo oscuro)
- Background: `rgba(255, 255, 255, 0.12)`
- Border: `1px solid rgba(255, 255, 255, 0.14)`
- Color: `#b9ebff`
- Texto strong: `#ffffff`

---

## Icon Wrappers
- Size: `48x48px`
- Border-radius: `12px`
- Background normal: `var(--color-bg-bento)`
- Color normal: `var(--color-primary)`
- Hover: background → `var(--color-primary)`, color → `#ffffff`, `translateY(-6px) scale(1.15) rotate(4deg)`

---

## Typography Patterns

### Section Heading
- Font: `var(--font-heading)` (Poppins)
- Size: `2.8rem`
- Weight: `800`
- Letter-spacing: `-0.03em`
- Color: `var(--color-navy)`

### Hero H1
- Font: display (Outfit) o heading (Poppins)
- Size: `4.5rem` / `clamp(2.5rem, 4.8vw, 4.8rem)`
- Weight: `800`
- Letter-spacing: `-0.04em` a `-0.05em`
- Line-height: `1.05`

### Gradient Text (highlight)
```css
background: var(--gradient-text);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
```

### Stat Number
- Size: `4rem`, weight `800`, color `var(--color-primary)` con gradient text

---

## Backgrounds

### Page Background Soft
```css
background:
  radial-gradient(circle at 15% 20%, rgba(69, 208, 255, 0.18), transparent 25%),
  radial-gradient(circle at 85% 15%, rgba(0, 100, 224, 0.18), transparent 22%),
  linear-gradient(180deg, #f8fbff 0%, #eef5ff 100%);
```

### Section Alternada
- `#ffffff` / `#fcfdff` / `var(--color-bg-soft)`
- Separadores: `1px solid var(--color-border)`

---

## Layout

- Max-width: `1360px`, centrado con `margin: 0 auto`
- Container padding: `24px` lateral
- Grids: 2 o 3 columnas con `gap: 24px–36px`
- Section padding-y: `80px–160px` (heroes más grandes)
