# SplashySound — Hero Cinematic Intro

Premium animated hero banner for Shopify, built for a waterproof RGB shower speaker.

## Files

| File | Description |
|------|-------------|
| `sections/hero-cinematic-intro.liquid` | Main Shopify section — drop onto homepage |
| `assets/hero-cinematic.css` | Optional CSS overrides |

## Installation

1. In your Shopify admin, go to **Online Store → Themes → Edit code**
2. Upload `sections/hero-cinematic-intro.liquid` into the `sections/` folder
3. Go to **Customize → Homepage**, click **Add section**, choose **Hero Cinematic Intro**
4. Upload your product PNG (transparent background) in section settings
5. Upload your logo (white version recommended)
6. Set your headline, sub-headline, CTA text and link
7. Save

## Animation sequence (15 seconds)

| Timestamp | Scene |
|-----------|-------|
| 0–2s | Black screen, background gradient fades in with floating particles |
| 2–5s | Product fades in with RGB ring; macro zoom begins |
| 5–8s | Water droplets appear on product surface; each reflects RGB colours |
| 8–12s | Shower streams fall in slow-motion; 180° orbital camera rotation |
| 12–14s | Product isolated with studio lighting; main headline reveals |
| 14–15s | End card — logo + sub-headline + CTA button |

## Customisation

All colours are CSS custom properties on `:root`:

```css
--hero-rgb-a: #ff0055;   /* magenta */
--hero-rgb-b: #00e5ff;   /* cyan    */
--hero-rgb-c: #a259ff;   /* violet  */
--hero-rgb-d: #00ff88;   /* green   */
```

Override them in your theme's `base.css` or in the **Custom CSS** field of the theme editor.

## Notes

- Uses Canvas 2D for all particle/water effects — no external dependencies
- Fully accessible: respects `prefers-reduced-motion`
- Loop mode available via section checkbox setting
- Replay button appears after the 15-second sequence
- Product image should be PNG with transparent background for the drop-shadow glow effect
