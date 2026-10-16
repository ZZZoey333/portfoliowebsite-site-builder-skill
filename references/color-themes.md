# Color theme presets

Themes change the visual treatment, not the page map or component structure. Ask which theme the user prefers, or use their supplied palette. Translate palette colors into semantic roles (page background, surface, text, primary action, accent) and check contrast for actual text sizes before implementation.

## Original portfolio theme

Extracted from the supplied source stylesheet `css/design-standards.css`:

| Role | Color | Notes |
|---|---|---|
| Primary | `#6610F2` | Source variable `--primary-color`; saturated violet used for links and primary actions. |
| Primary hover | `#510BC4` | Source variable `--primary-hover`. |
| Main text | `#212529` | Dark neutral text. |
| Secondary text | `#6C757D` | Muted text. |
| Page background | `#FFFFFF` | White canvas. |
| Light surface | `#F8F9FA` | Pale neutral surface. |
| Border | `#DEE2E6` | Neutral separators and borders. |

This documents the source's default design variables. The source project also contains alternate color stylesheets; do not infer that every page uses an identical palette unless verified.

## Blue, Dark Blue, Green, Light Blue

Palette provided by the portfolio author as a preferred alternative. Hex values are transcribed from the supplied image.

| Palette color | HEX | Suggested semantic role |
|---|---|---|
| Blue | `#136CFC` | Primary links, buttons, selected states. Use white text only after contrast verification for the actual size and weight. |
| Dark Blue | `#152641` | Main text, dark navigation/footer areas, strong headings. |
| Green | `#C3F84A` | Highlight/accent for small surfaces, tags, active markers, or decorative details. Avoid using it for small text on a light background. |
| Light Blue | `#E8F4FC` | Page background or soft section surface. |

Suggested application: use Light Blue as a soft canvas, Dark Blue for text and structural elements, Blue for interactive emphasis, and Green sparingly for contrast and energy. Do not give every color equal visual weight. Validate text and control contrast in context; palette membership alone does not guarantee accessible contrast.

## Adding another palette

For each new theme, record its source or author, color names and HEX values, suggested semantic roles, and any contrast limitations. Prefer palette references as inspiration; do not copy another creator's page layout, branding, or assets. Re-check current accessibility contrast against the actual foreground/background pairings before shipping.
