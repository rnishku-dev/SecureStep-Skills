---
name: ssp-website-design-art-directions
description: Create or refine websites with a business-specific visual identity, consistent typography, and whole-number font sizes. Use when building a website or removing a generic AI-generated appearance. Preserve existing brand choices and requested scope.
---

# SSP Website Design Art Directions

Create a coherent website whose content, composition, and details fit the business. Avoid replacing one recognizable generated template with another. The user's brief and existing brand take precedence over suggested aesthetics.

## Establish direction

Inspect the relevant implementation, available brand assets, actual copy, and rendered site when available. Distinguish a focused refinement from a requested redesign. Preserve existing identity and working behavior for refinements; do not expand the assignment into a full redesign.

Before implementation, briefly state the audience, primary visitor task, visual direction, and typography and layout approach. Use supplied references to identify specific qualities worth adapting, rather than copying an unrelated site's structure wholesale.

Proceed with reasonable, stated assumptions when context is sufficient. Ask only when a missing decision would materially affect the result. Do not require a fixed brief form or create planning documents for every small edit.

## Typography invariants

- Use one primary font family. Add at most one complementary display family when it provides a clear benefit; monospace is reserved for content such as code that needs it.
- Preserve an established brand typeface where appropriate. Do not automatically replace system fonts or select from a fixed list of fashionable fonts.
- Define shared styles for display text, heading levels, body text, navigation, buttons, inputs, labels, and captions. Equivalent roles across comparable pages must use consistent family, size, weight, and line height.
- Make buttons and form controls inherit the intended font. Specify suitable fallbacks and load only the font weights actually needed.
- Author font-size tokens and overrides in whole-number CSS pixels: use 12px, 16px, or 48px, never 12.2px or 47.6px. Equivalent rem values are acceptable when they represent whole-number pixel sizes at the default root size. Do not force the root font size or disable user scaling to achieve this.
- Prefer discrete whole-number font sizes at responsive breakpoints. Avoid fluid font-size interpolation, viewport-based sizing, and transforms that scale text when they undermine this requirement. Browser zoom, device scaling, and user font settings may produce fractional rendered values; do not counteract them.
- Whole-number font sizing does not prohibit proportional line heights, rem notation, fractional layout dimensions, or letter spacing. Do not apply the integer rule indiscriminately to all CSS values.
- Choose a limited scale for the content. An optional starting scale is 12, 14, 16, 18, 24, 32, 40, 48, and 64px. Use only the sizes needed; body text must remain comfortably readable.
- Build hierarchy with weight, spacing, placement, and size. Avoid tiny supporting text or enormous headings merely to create dramatic contrast. Check long headings and missing-font fallbacks on mobile.

## Art direction and layout

Use reusable tokens for typography, color, spacing, borders, radii, and shadows. Assign colors clear roles and use a consistent spacing rhythm. Equivalent components should look and behave consistently.

Question automatic use of purple gradients, gradient headings, floating rounded cards, decorative icon circles, repeated pills, three identical feature cards, and centered content in every section. These are patterns to evaluate, not universal bans. Retain them when they serve the content, established brand, or interaction.

Do not prescribe parchment backgrounds, serif headlines, orange accents, dark industrial palettes, or oversized typography as universal replacements. Choose the visual direction for this project.

Let information determine section order and layout. Use lists for scanning, tables for comparisons, steps for processes, screenshots or diagrams for explanation, and cards for distinct grouped items. Keep content outside containers when a container adds no value. Vary composition when it improves understanding; retain familiar navigation and interaction conventions.

For marketing pages, prioritize credibility and a clear next action. For applications, prioritize task completion and scanability. For articles and documentation, prioritize comprehension and reading comfort. Apply visual expression in proportion to the surface's purpose.

## Content and assets

Use clear, natural wording tied to the actual business and supplied evidence. Prefer concrete descriptions over vague promises and repeated slogans. Use paragraphs, descriptive headings, and meaningful action labels. Avoid em dashes in authored copy.

Do not invent customer logos, testimonials, certifications, awards, statistics, or capabilities. Preserve factual copy during visual refinements unless rewriting is requested. Flag missing or unverified material; do not present placeholders as real proof.

Use relevant supplied photography, product screenshots, and brand assets. Introduce new imagery only when it improves understanding or supports the chosen direction. Avoid decorative images and icons that communicate nothing.

## Implementation and review

Use the existing stack and component conventions. Make responsive layouts, semantic headings, accessible labels, visible keyboard focus, readable contrast, and practical touch targets part of implementation. Respect browser zoom and reduced motion preferences.

Keep links, buttons, navigation, and forms functional within the requested scope. Include loading, empty, success, and error states where the requested interaction needs them. Do not build an unrequested backend or replace established behavior to demonstrate a design.

For browser activity, use Microsoft Edge. Inspect desktop and mobile together in a bounded review pass. Check typography consistency, authored integer font sizes, hierarchy, spacing, contrast, image relevance, overflow, long content, interaction states, and the primary user journey. Fix observed defects in one batch and confirm the affected areas. Avoid indefinite polishing.

Inspect relevant styles and rendered output together: font declarations alone do not prove that the intended font loaded. Verify the actual font where browser tools permit. If browser verification cannot run, state that limitation rather than claiming visual validation.

Report the implemented result, relevant verification, and remaining limitations. Creation or refinement does not authorize publication, deployment, or changes to client data. Keep client work read-only until a human approves changes, and explain the impact of a proposed client change.
