# Ikigai Creative — Design System

**Version 1.0**
*A brand is a promise your customers feel.*

This is the single source of truth for the Ikigai Creative identity. It exists so every asset, page, and deck holds together, whether it is built by Alex, a junior designer, or Claude Code. Where this document and any older file disagree, this document wins.

Companion file: `design-system.html` renders every token, mark, and component in the browser. Use it as the visual reference. Use this markdown as the spec you paste into builds.

---

## 1. The idea

**Engineer's brain, storyteller's heart.**

The two koi are the whole brand in one image. The teal fish is the discipline that makes a brand hold together: structure, precision, repeatability. The terracotta fish is the warmth that makes people care: feeling, motion, a point of view. Every choice in this system balances the two.

**Personality:** a steady creative partner. Calm and human-centered, with sparks of joy. Earthy and timeless, refined but approachable, slightly premium.

**Traits:** Calm. Precise. Motivational. Human-centered. Lightly playful.

---

## 2. Logo suite

Six approved lockups. The rule is simple: match the mark to its background so the koi disc always contrasts. The koi carry the brand, so give them room and never redraw them.

| Mark | File | Use it for |
|------|------|-----------|
| Primary horizontal lockup | `ikigai_creative_Koi_Center_2000x.png` | Wide spaces. Site header, deck covers, email footer. Wordmark splits around the koi. |
| Badge lockup, light | `IC_Logo_Lockup_on_Light_BG_2000x.png` | Koi badge beside the wordmark, on Soft Sand or white. |
| Badge lockup, dark | `IC_Logo_Lockup_on_Dark_BG_2000x.png` | Reversed wordmark on Oxford Blue or photography. |
| Koi badge, dark circle | `Dark_Logo_2000x.png` | Oxford Blue disc. Use on light surfaces. Avatars, favicons, stamps. |
| Koi badge, sand circle | `Light_Logo_2000x.png` | Soft Sand disc. Use on dark surfaces where the dark badge would disappear. |
| Stacked logomark | `IC_Stacked_Text_logomark_2000x.png` | IKIGAI over creative with the koi tail. Square and tall formats. |

### Clear space and size
- Keep clear space on all sides equal to the height of the koi badge.
- Do not scale the badge lockups below 120 px wide, or the horizontal lockup below 200 px wide. Below that, use the koi badge alone.

### Do
- Choose the mark whose disc contrasts with the background.
- Scale the whole lockup as one unit.
- Reproduce from the master files only.

### Do not
- Recolor the koi or the wordmark, or introduce off-palette colors.
- Stretch, rotate, skew, or add drop shadows and outlines.
- Place the dark-circle badge on a dark field, or the sand-circle badge on a light field.
- Rebuild the wordmark in a different typeface.

---

## 3. Color

Warm and cool in balance, the same duality as the koi. Deep Teal leads, Clay Terracotta answers, Sunflower Yellow sparks, and the neutrals let the work breathe.

### Core palette

| Name | Hex | RGB | Role |
|------|-----|-----|------|
| Deep Teal | `#1C6B6B` | 28, 107, 107 | Primary. Calm confidence and professionalism. Headlines, primary buttons, links. |
| Clay Terracotta | `#D76B42` | 215, 107, 66 | Secondary. Earthy warmth, human connection. Accents, the wordmark, secondary CTAs. |
| Sunflower Yellow | `#F5B82E` | 245, 184, 46 | Highlight. Optimism, energy, creativity. Use sparingly. |
| Oxford Blue | `#003A5C` | 0, 58, 92 | Deep anchor. The badge disc and darkest surfaces. Grounds the warm tones. |
| Charcoal Slate | `#2E2E2E` | 46, 46, 46 | Primary text and grounding. Steadier than pure black. |
| Soft Sand | `#F4F1EB` | 244, 241, 235 | Warm neutral background. Softer than white. The default canvas. |

### Extended scales

Sampled directly from the koi gradients so tints and shades stay true to the artwork.

**Teal:** `#1C6B6B` → `#2E8A8A` → `#5CC2C3` → `#A3DBE2` → `#E7F3F3` (wash)
**Terracotta:** `#C55C3B` → `#D76B42` → `#E58468` → `#F18D79` → `#FBEEE8` (wash)
**Sunflower wash:** `#FDF4DC`

### Functional tokens
- Text / ink: `#2E2E2E`
- Muted text: `#6E6A63`
- Hairline / border: `#E4DED2`
- Surface (card): `#FFFFFF`

### Contrast rules
- Deep Teal on white, Oxford Blue on Soft Sand, and Charcoal on Soft Sand all pass WCAG AA. These are your safe text pairings.
- Sunflower Yellow does not pass text contrast on white or sand. Use it as a fill or highlight only, and set any text on it in Charcoal, never white.
- Terracotta on white passes for large text and UI, not for long body copy. Keep it to accents and short lines.

---

## 4. Typography

Three faces, three clear jobs. Rounded and human for the voice, neutral and readable for the work, italic and distinct for the name.

| Role | Family | Notes |
|------|--------|-------|
| Display / headlines | **Avenir Next Rounded** | Calm, modern, human. Professional but soft. Weights 600 to 700. Licensed brand font. |
| Body / interface | **Inter** | Highly readable, neutral, balanced. All paragraphs, labels, captions, controls. Weights 400, and 500 to 600 for emphasis. |
| Wordmark only | **Omnes SemiCond, Medium Italic** | The wordmark lockup. SemiBold is the approved alternate. Reference size 430 pt. Never used for headlines or body. |

Fallback stacks for the web, where the licensed faces are not installed:
- Display: `"Avenir Next Rounded", "Avenir Next", Nunito, ui-rounded, system-ui, sans-serif`
- Body: `"Inter", system-ui, -apple-system, sans-serif`

### Type scale

| Token | Size | Line height | Weight | Family |
|-------|------|-------------|--------|--------|
| Display XL | 56 px | 1.05 | 700 | Display |
| Display | 40 px | 1.10 | 700 | Display |
| H1 | 32 px | 1.15 | 700 | Display |
| H2 | 24 px | 1.20 | 600 | Display |
| H3 | 20 px | 1.30 | 600 | Display |
| Body | 17 px | 1.60 | 400 | Body |
| Small | 15 px | 1.50 | 400 | Body |
| Caption | 12 px | 1.40 | 600 | Body, uppercase, letter-spacing .12em |

---

## 5. Foundations

**Spacing** runs on a 4 px base: 4, 8, 12, 16, 24, 32, 48, 64, 96.

**Radius:** small 8 px, base 14 px, large 24 px, pill 999 px. The brand is soft, so nothing is sharp-cornered by default.

**Elevation:** keep shadows low and warm.
- `shadow-sm`: `0 1px 2px rgba(0,58,92,.05)`
- `shadow`: `0 1px 2px rgba(0,58,92,.04), 0 10px 30px rgba(0,58,92,.07)`

---

## 6. Components

- **Buttons** carry the display face, weight 700, pill radius. Primary is Deep Teal on white text. Secondary is Terracotta on white. Ghost is a Deep Teal 2 px inset border on transparent. Sunflower buttons take Charcoal text.
- **Cards** sit on white with a hairline border, 24 px radius, and the base shadow. A terracotta uppercase kicker labels the card.
- **Form fields** sit on Soft Sand, border to the hairline color, and focus to Deep Teal with a soft teal focus ring. Labels are plain and name what they collect.
- **Pills / tags** use the wash tints: teal wash for owned terms, sunflower wash for highlights.

---

## 7. Voice

A mentor, not a textbook. Confident and warm, precise over inflated. Short punchy lines mixed with longer reflective ones. PSL structure where it fits: Problem, Solution, Lesson.

**Own:** clarity, systems, trust, feel, build, behave, promise.
**Avoid:** synergy, leverage, world-class, disrupt, cutting-edge, solutions.

**One hard rule: no em dashes, anywhere.** Use a comma, a period, or a restructured sentence. No filler language.

Before: *We leverage cutting-edge, world-class creative solutions to disrupt your market.*
After: *We turn complexity into a brand people trust. Then we build the system that keeps it consistent.*

---

## 8. Build-ready token block

Paste this into any Claude Code build (it fills Input 3 of the Website Build-Out Brief). Colors and type map one to one with the tables above.

```css
:root{
  /* Core brand */
  --oxford:#003A5C;
  --teal:#1C6B6B;
  --teal-mid:#5CC2C3;
  --teal-light:#A3DBE2;
  --teal-wash:#E7F3F3;
  --terra:#D76B42;
  --terra-deep:#C55C3B;
  --terra-salmon:#F18D79;
  --terra-wash:#FBEEE8;
  --sun:#F5B82E;
  --sun-wash:#FDF4DC;
  --sand:#F4F1EB;
  --charcoal:#2E2E2E;

  /* Functional */
  --ink:#2E2E2E;
  --muted:#6E6A63;
  --line:#E4DED2;
  --surface:#FFFFFF;

  /* Type */
  --font-display:"Avenir Next Rounded","Avenir Next",Nunito,ui-rounded,system-ui,sans-serif;
  --font-body:"Inter",system-ui,-apple-system,sans-serif;
  --font-word:"Omnes SemiCond","Avenir Next",Nunito,sans-serif;

  /* Spacing */
  --space-1:4px; --space-2:8px; --space-3:12px; --space-4:16px;
  --space-5:24px; --space-6:32px; --space-7:48px; --space-8:64px; --space-9:96px;

  /* Shape */
  --radius-sm:8px; --radius:14px; --radius-lg:24px; --radius-pill:999px;
  --shadow-sm:0 1px 2px rgba(0,58,92,.05);
  --shadow:0 1px 2px rgba(0,58,92,.04), 0 10px 30px rgba(0,58,92,.07);
}
```

---

*Ikigai Creative · Design System v1.0 · alex@ikigaicreative.xyz · ikigaicreative.xyz*
