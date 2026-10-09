# Changelog

## [Unreleased]

## [1.0.1](https://github.com/genskyff/obsidian-arkfield/releases/tag/1.0.1) - 2026-10-09

### Fixed

- The active tab in the Settings sidebar is now shaded with the same gray tint as active items in the file list and outline, instead of keeping the paper background that made it hard to distinguish on desktop ([1cc0960](https://github.com/genskyff/obsidian-arkfield/commit/1cc0960)).

## [1.0.0](https://github.com/genskyff/obsidian-arkfield/releases/tag/1.0.0) - 2026-10-09

### Added

- Arkfield for Obsidian, a light theme ported from [Arkfield for Typora](https://github.com/genskyff/typora-arkfield): paper-white notes on a faint engineering grid, charcoal ink, signal-yellow accents, square corners and hard offset shadows. Requires Obsidian 1.14.4 or later. ([8468e7f](https://github.com/genskyff/obsidian-arkfield/commit/8468e7f))
- Styling for the whole document surface in Reading view and Live Preview: inline title, headings 1–6 with signal rules and bars, body text, links and wikilinks, tags, lists and task lists, blockquotes, callouts, tables, inline and fenced code, math, Mermaid, note properties, footnotes, embeds, and HTML details, definition lists and ruby.
- Bullets cycle filled circle, open circle and square by nesting depth and now match between Reading view and Live Preview down to the sixth level ([6691726](https://github.com/genskyff/obsidian-arkfield/commit/6691726)), and checked checkboxes keep their ink border when hovered ([704ac59](https://github.com/genskyff/obsidian-arkfield/commit/704ac59)).
- Callouts keep GitHub's icons and colors for NOTE, TIP, IMPORTANT, WARNING and CAUTION, with CAUTION colored separately from WARNING (Obsidian aliases the two by default).
- App shell styling: the active note tab carries a signal-yellow rule that wipes in when you switch tabs, plus styled sidebars and file explorer, outline, command palette, menus, modals, popovers, notices, status bar and visible focus outlines for keyboard navigation.
- Three variable fonts are embedded in `theme.css`: Inter for text and interface, Space Grotesk for headings and technical labels, Fira Code for code. CJK text falls back to the system font stack.
- PDF export handles pagination: headings stay clear of page breaks, code blocks wrap instead of overflowing, long tables repeat their header row, and bold highlights print as an opaque yellow band rather than a translucent gradient ([fb3cf11](https://github.com/genskyff/obsidian-arkfield/commit/fb3cf11)). `<div style="page-break-after: always;"></div>` shows a `PAGE BREAK` marker in Reading view and is not printed.
- Dark mode has no dedicated palette: Arkfield's rules and signal yellow are layered on top of Obsidian's default dark colors.
- Narrow panes and phones get smaller headings, and animations are disabled under `prefers-reduced-motion`.
- Releases attach `manifest.json` and `theme.css` next to `arkfield-<version>.zip`, and tags use the plain version (`1.0.0`) because Obsidian resolves a theme release by the version in its manifest ([a1cd678](https://github.com/genskyff/obsidian-arkfield/commit/a1cd678), [18b7314](https://github.com/genskyff/obsidian-arkfield/commit/18b7314)).
- An English README and a showcase note (`assets/coverage.md` with `assets/coverage-figure.svg`) document the theme and let you check formatting and mixed Chinese, Japanese and English text inside a vault ([764ef29](https://github.com/genskyff/obsidian-arkfield/commit/764ef29)).
