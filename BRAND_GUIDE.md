# MyPeppers Brand Guide

## Brand idea

MyPeppers is a private health and routine tracking app designed with women in mind. The brand should feel calm, capable, organized, and supportive. It is a tracking companion—not a doctor, pharmacy, treatment service, or medical authority.

Core line: **Your whole routine, in one private place.**

## Logo system

The current mark is an original temporary SVG concept requiring final brand-design review before trademark filing or broad commercial rollout.

It combines:

- an abstract, inclusive woman's profile;
- a circular path representing recurring routines;
- a connected tracking line and three data points.

It intentionally avoids fertility-only, pregnancy-only, beauty, food, pharmaceutical, and anatomical imagery.

Available implementations:

- `src/components/BrandLogo.astro` — reusable header, footer, mobile, icon-only, light, and monochrome lockups;
- `public/brand-mark.svg` — red standalone mark;
- `public/favicon.svg` — small browser icon;
- `public/social-profile.svg` — red-on-white social profile concept;
- `public/app-icon-concept.svg` — white-on-red app icon concept.

Maintain clear space around the mark equal to at least one tracking-dot diameter. Do not stretch, rotate, add shadows to, recolor outside the approved palette, or separate the profile from the tracking line.

## Color palette

All website colors are centralized as CSS custom properties in `src/pages/index.astro`.

| Role | Token | Value | Use |
|---|---|---:|---|
| Primary red | `--red-primary` | `#C9363E` | Primary CTAs, icons, selected states |
| Deep red | `--red-deep` | `#8F1F28` | Headline accents, hover states, footer |
| Bright red | `--red-bright` | `#E64B52` | Small non-text highlights and focus rings only |
| White | `--white` | `#FFFFFF` | Main surfaces and cards |
| Warm white | `--warm-white` | `#FFF9F8` | Main background and alternating sections |
| Very light red | `--red-soft` | `#FCEBEC` | Selected items and quiet section backgrounds |
| Charcoal | `--charcoal` | `#2B2526` | Primary body copy |
| Muted gray | `--muted` | `#6F6466` | Secondary copy |
| Light border | `--border` | `#EADDDD` | Rules, card borders, form controls |

Do not introduce alternate primary palettes. Red should remain purposeful rather than decorative.

## Accessibility and contrast

Verified WCAG contrast ratios:

- Primary red on white: **5.15:1** — passes AA for normal text.
- Deep red on white: **8.77:1** — passes AAA for normal text.
- Charcoal on white: **15.05:1** — passes AAA.
- Charcoal on warm white: **14.45:1** — passes AAA.
- Muted gray on white: **5.69:1** — passes AA.
- Deep red on very light red: **7.61:1** — passes AAA.

Bright red on white is **3.82:1**. Use it only for large graphics, icons, focus rings, and non-text decoration—not normal-sized text or white-button backgrounds.

## Typography

Use the privacy-conscious system font stacks already defined in the site:

- Editorial headings: `Iowan Old Style`, `Palatino Linotype`, `Book Antiqua`, `Palatino`, `Georgia`, serif.
- Interface and body copy: `Inter` when locally available, then the native system sans-serif stack.

Do not load remote font services solely for brand styling.

## Icon system

`src/components/LineIcon.astro` contains the red line-icon system for:

- peptides and injectables;
- prescriptions;
- antidepressants and mental-health medications;
- supplements;
- symptoms;
- menstrual-cycle tracking;
- perimenopause and menopause;
- sleep;
- mood;
- appointment summaries;
- privacy.

Icons use a consistent 24px view box, rounded line caps, and 1.65px strokes. They inherit color from their container and should normally use primary red on white.

## Voice and imagery

Use clear, reassuring language such as “notice patterns” and “prepare clearer notes.” Never imply diagnosis, treatment, guaranteed results, hormone balancing, weight-loss outcomes, or medical authority.

Prefer app-screen previews, timeline rhythms, and connected routine points. Avoid stock-photo clichés, dominant syringe imagery, hospital imagery, and before-and-after visuals.
