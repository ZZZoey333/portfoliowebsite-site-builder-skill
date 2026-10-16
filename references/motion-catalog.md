# Named motion catalog

Names are shared prompt vocabulary. Each recipe describes an intent and visible result; it does not mandate a particular animation library. Keep durations and distances restrained, avoid motion that competes with reading, and preserve all essential information without animation.

| Name to use in prompts | Behavior | Good places to use it | Source behavior |
|---|---|---|---|
| **Reveal Up / 滚动上浮渐入** | Element fades in while moving upward a short distance when it enters the viewport. | Section headings, intro text, project cards. | `fadeInUp` triggered by WOW on `.wow` elements. |
| **Section Divider Reveal / 分隔线显现** | Decorative divider appears with a short upward reveal. | Below section headings. | `slideInUp` with a small stagger delay. |
| **Staggered Reveal / 错峰进入** | Related items reveal in sequence with small delays. | Heading eyebrow → title → divider; card rows; grouped skills. | `data-wow-delay` values stagger `fadeInUp`/`slideInUp`. |
| **Sticky Nav Slide-In / 吸顶导航滑入** | After scrolling past the opening area, navigation becomes fixed/sticky and slides into its compact state. | Shared site header. | `sticky-top-slide`; `.primary-menu` gains `sticky-on` after a scroll threshold. |
| **Smooth Anchor Scroll / 锚点平滑滚动** | Clicking an in-page navigation link scrolls smoothly to the matching section. | One-page portfolios and long case studies. | `.smooth-scroll` animates document scroll. |
| **Dropdown Slide / 下拉菜单展开** | Navigation submenu opens with a brief slide transition and closes when dismissed or focus moves away. | Desktop navigation with nested destinations. | jQuery `slideDown`/`slideToggle`; provide equivalent keyboard/touch behavior. |
| **Gallery Carousel / 作品画廊轮播** | A horizontal gallery advances between related images or steps, with clear controls and position cues. | Process screens, UI galleries, journey steps. | Owl Carousel instances with page-specific settings. |
| **Portfolio Filter / 作品分类筛选** | Selecting a category updates the visible project cards and selected filter state. | Project listing when categories are useful. | `.portfolio-menu` selection and portfolio filtering. |
| **Back-to-Top Reveal / 返回顶部按钮显现** | A return-to-top control appears after scrolling down; activating it scrolls to the page start. | Long pages. | Control visibility after scroll threshold and smooth scroll to top. |
| **Modal Fade / 模态窗淡入** | A dialog appears above the page with a fade transition and can be dismissed accessibly. | Policies, image detail, optional contact flow. | Bootstrap `.modal.fade`. |

## Prompt format

Users can request a motion by name and specify target, trigger, strength, and reduced-motion behavior:

> Apply **Staggered Reveal** to the case-study section heading and three project cards. Start when each group enters the viewport, keep the stagger subtle, and disable the movement for users who prefer reduced motion.

If a requested effect is ambiguous, clarify what triggers it and which element should move. Do not infer that an effect name implies a specific third-party library.

## Motion implementation notes

- Support `prefers-reduced-motion: reduce`; remove or greatly reduce nonessential movement while keeping elements visible.
- Ensure animated elements do not begin hidden if JavaScript fails or motion is disabled.
- Avoid animating large layout dimensions or repeatedly moving text while the user reads.
- Carousels need labeled previous/next controls, a visible current state where appropriate, and usable touch/keyboard controls. Avoid automatic movement unless the user requests it and can pause it.
- Dropdowns and dialogs need keyboard operation, focus handling, and accessible state announcements; visual transitions alone are not interaction behavior.
