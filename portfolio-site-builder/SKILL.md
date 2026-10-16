---
name: portfolio-site-builder
description: Help beginners and designers plan, build, or improve a personal UI/UX portfolio website using reusable page sections, project case-study patterns, and named motion recipes. Use when creating a portfolio site or translating a portfolio brief into pages and components.
---

# Personal Portfolio Site Builder

Help the user turn their own background and work into a clear, reusable portfolio website. The reference system is based on a real multi-page UI/UX portfolio, but its visual identity is optional: preserve the user's chosen style and use the reference structure only where it fits.

## Workflow

1. Establish the user's audience, role, portfolio content, preferred stack (if any), and whether they want a single-page or multi-page site. For beginners, recommend a simple implementation and explain tradeoffs in plain language.
2. Propose a page map and section order before filling it with invented biography or project facts. Ask for missing content when it changes the story; otherwise use clearly marked placeholders.
3. Build the shared shell and reusable sections described in [references/page-patterns.md](references/page-patterns.md). Make project case studies configurable: users can include, omit, and reorder the relevant sections.
4. Offer named motion recipes from [references/motion-catalog.md](references/motion-catalog.md). Describe the visible behavior in plain language, then implement the chosen recipe with the user's stack. Do not add every motion by default; use motion to clarify hierarchy or interaction.
5. Apply the user's visual direction consistently across typography, color, spacing, imagery, and components. The reference site's palette is only one starting theme; themes can change without changing page structure.
6. Make layouts responsive and interactions usable with keyboard and touch. Respect reduced-motion preferences, provide visible focus states, and keep essential content available when animation is disabled.
7. Summarize the pages/components and named motions delivered, and point out any content the user still needs to supply.

## Reusable design principles

- Lead with the person's role and value, then make selected work easy to find.
- Keep the home page a concise introduction and gateway; let each case study carry its own narrative and evidence.
- Use a consistent section-heading pattern, spacing scale, navigation, footer, and project-card system.
- Let project pages share a flexible sequence rather than forcing every project into identical content.
- Keep motion subtle, purposeful, and consistent. A motion name describes a reusable behavior, not a required library or exact implementation.
- Do not copy reference copy, personal data, project claims, imagery, or source code into a new user's site. Ask for their own material or use labeled placeholders.

## References

- Read [references/page-patterns.md](references/page-patterns.md) when planning the site map or building page and case-study sections.
- Read [references/motion-catalog.md](references/motion-catalog.md) when the user asks to choose, name, or implement motion.
