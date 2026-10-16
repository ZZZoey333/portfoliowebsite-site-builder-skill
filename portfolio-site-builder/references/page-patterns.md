# Page and section patterns

These patterns were extracted from the supplied portfolio source. Treat them as reusable content structures, not fixed visual layouts. A user may combine them into one page or split them across routes.

## Shared site shell

- **Primary navigation**: links to Home, Projects, About, and Contact; indicate the active destination. On small screens, use a clearly labeled menu toggle.
- **Section heading**: optional eyebrow/descriptor, main heading, and short decorative divider. Use the same hierarchy throughout.
- **Footer**: name or wordmark, relevant navigation/social links, copyright or attribution if applicable.
- **Back-to-top control**: optional on long pages; show after meaningful scrolling and give it an accessible name.
- **Contact call-to-action**: optional closing section on the home page, project listing, and case studies.

## Home page

Suggested order:

1. **Hero / personal introduction**: name, role, concise value statement, portrait or visual, and one or two actions (view work, contact).
2. **About preview**: short introduction, approach or strengths, and a link to the full About page.
3. **Services or capabilities**: a small set of clear disciplines, each with a short explanation. Omit if it does not help the user's positioning.
4. **Featured projects**: selected project cards linking to their case studies.
5. **Contact invitation**: an approachable prompt and direct contact action.
6. **Footer**.

## Project listing

- Page heading and optional one-line context.
- Optional category filters when there are enough projects to justify them. Filters must work by keyboard and touch and expose the selected state.
- Project grid/list. Each card should show a meaningful image, project name, category or role, and a link with a clear accessible label.
- Optional contact invitation and shared footer.

## Project card

Make the full card's purpose clear without requiring hover. Include a thumbnail/cover, title, discipline or tags, and an explicit link. Avoid placing unrelated nested links inside a single clickable card.

## Case-study page

Use a flexible sequence; include only sections supported by the project material:

1. **Project hero**: project title, discipline, short summary, and cover image/media.
2. **Project snapshot**: role, team, duration, tools, scope, and constraints where known.
3. **Context and challenge**: the situation, audience, and problem being addressed.
4. **Research and insights**: methods, evidence, and resulting insights. Do not present unsupported claims as research findings.
5. **Design direction / concept**: principles, concept, or strategy.
6. **Process and iterations**: key decisions, explorations, tests, and what changed.
7. **Solution / interface showcase**: screens, prototypes, service journey, video, or image gallery. Use a carousel only when it improves browsing; otherwise show images in a readable sequence.
8. **Outcome and reflection**: measured outcomes when available; otherwise describe qualitative results and lessons without inventing metrics.
9. **Next/previous project and contact prompt**.

The source portfolio uses distinct compositions: some case studies foreground service-design research and flows; others foreground interface screens, gameplay/video, or visual assets. Preserve that flexibility.

## About page

- Short professional introduction and point of view.
- Relevant education and experience, in a scannable timeline or grouped list.
- Skills grouped by practice (for example research, design, prototyping, tools) rather than an unstructured keyword dump.
- Optional selected projects, resume link, and contact action.

## Contact page

- Clear invitation and preferred contact method(s).
- Email and professional/social links supplied by the user.
- Optional response expectations or a short form, with clear labels and feedback if a form is used.

## Content model for reuse

For a portfolio builder, store repeated content as data where the chosen stack supports it:

- Site identity: name, role, intro, portrait, links.
- Navigation items.
- Capabilities: title, explanation, optional icon.
- Projects: slug, title, summary, category, cover, role, metadata, and ordered case-study sections.
- Contact details and footer links.

Do not require a framework or data model when the user is building a very small static site; reuse the content structure conceptually.
