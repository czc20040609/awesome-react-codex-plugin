---
name: react-frontend-development
description: Use for every React or React Native frontend task, including building, modifying, debugging, refactoring, reviewing, testing, styling, component selection, architecture decisions, and learning; consult the bundled Awesome React catalog and verify current APIs with official documentation.
---

# React Frontend Development

Treat this as the default working mode for React and React Native frontend tasks. Use the bundled `references/awesome-react.md` catalog as a discovery index, not as a substitute for understanding the user's codebase or checking current official documentation.

## Before changing code

1. Inspect the existing project before choosing an approach: `package.json`, lockfile, framework, routing, styling system, component library, state/data layer, entry points, tests, and local conventions.
2. Preserve the project's existing architecture and visual language. Reuse installed components and utilities before introducing a new dependency or pattern.
3. Identify the user's platform and rendering target: React web, a specific framework, React Native, or another renderer. Do not apply web DOM/CSS assumptions to React Native.
4. Translate the request into concrete behavior and acceptance criteria. When the user asks for implementation, implement the change rather than only listing recommendations.

## Frontend implementation standards

- Build semantic, accessible UI: correct HTML or native primitives, keyboard/focus behavior, labels, useful error messages, sufficient contrast, and sensible screen-reader output.
- Cover meaningful UI states: loading, empty, error, success, disabled, pending, and slow or partial data where applicable.
- Keep state ownership explicit. Prefer the smallest state surface, stable props, predictable effects, and clear data-fetching boundaries. Avoid unnecessary global state and effect chains.
- Match the repository's TypeScript, linting, formatting, testing, and styling conventions. Do not introduce `any` or a new styling system without a reason.
- Keep components composable and responsive. Separate domain/data concerns from presentation when that improves reuse, but do not create abstractions without a concrete caller.
- Consider performance when it matters: render cost, list virtualization, bundle size, image loading, memoization, and server/client boundaries. Measure or explain assumptions instead of cargo-culting optimizations.
- Preserve security and correctness at boundaries: validate external data, handle asynchronous cancellation or stale responses, and do not trust user-controlled HTML or URLs.

## Using the Awesome React catalog

1. Search the relevant headings and links in `references/awesome-react.md` when selecting a framework, component library, state/data tool, router, form solution, testing tool, chart, map, renderer, animation library, or React Native package.
2. If comparing options, give a short decision-oriented shortlist. For each option, state what it is good at, the main tradeoff, and the situation where it fits best. Do not call one option universally best without selection criteria.
3. Treat the catalog as a snapshot. Versions, maintenance, compatibility, licensing, pricing, API shape, and framework support can change. Verify those details against the resource's current official documentation or repository when they affect the decision.
4. If the catalog does not cover the request, say so plainly and use current authoritative sources if browsing is available. Never imply that an item is in the catalog when it is not.
5. For implementation questions, use the selected resource's current official documentation for API details and provide a minimal example that matches the project's actual stack.

## Learning and review mode

When the user is learning or asks for an explanation:

- Explain the relevant React concept in the context of the user's code, not as an isolated textbook definition.
- Show the smallest useful example, then identify the production concerns and common failure modes.
- Explain why the chosen component/library pattern fits and what tradeoff it introduces.

When reviewing or debugging:

- Reproduce or trace the behavior from the component boundary through state, effects, data fetching, styling, and rendering.
- Separate confirmed causes from hypotheses.
- Recommend a narrow fix first, then mention broader refactors only when they are necessary.

## Verification checklist

- Run the project's relevant formatter, linter, type checker, unit/component tests, and build when available and proportionate to the change.
- Check responsive behavior and interaction states when visual tooling is available; do not claim visual verification that was not performed.
- Report changed files, checks run, and any remaining uncertainty. Distinguish source changes, successful builds, and actual browser/device behavior.
- If a new dependency is genuinely required, explain why it is needed and use the project's package manager and lockfile conventions.

If the user has not supplied enough context, make a reasonable default assumption and state it briefly. Ask a follow-up only when the missing constraint would materially change the implementation.

## Scope and attribution

The reference file is a snapshot of [enaqx/awesome-react](https://github.com/enaqx/awesome-react), captured from commit `e6fd973eefe57d288a60e6d21bb9d8f343addfe9`. It is a starting index, not a guarantee of maintenance status or endorsement. Preserve the upstream links when referring users to a resource.
