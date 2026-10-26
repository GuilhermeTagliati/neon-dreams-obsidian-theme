<h1 align="center">Neon Dreams</h1>
<h3 align="center">Personal theme for <a href="https://obsidian.md">Obsidian</a></h3><br>

<p align="center"><img src="assets/banner.svg" width="680"></p>

## Preface

![Downloads|199](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Freleases.obsidian.md%2Fstats%2Ftheme&query=%24.Neon%20Dreams.download&style=for-the-badge&logo=obsidian&label=downloads&labelColor=%23131922&color=%236675ff)
![License](https://img.shields.io/badge/license-MIT-6675ff?style=for-the-badge&labelColor=%23131922)

A night-terminal Obsidian theme for personal knowledge management, journaling, project tracking and markdown-based workflows. Almost-black navigation, graphite reading surfaces, monospace titles and luminous cyan signals in dark mode; cool white and deep cyan in light mode. Custom link/action accents remain supported.

Backgrounds and interactive accents use configurable HSL tokens. Note titles remain neutral; cyan section headings use a separate signature hue. Semantic colors stay independent, so changing the accent does not turn every surface into a competing signal.

## Refactoring UI Refinement

Version 1.2.0 makes the hierarchy more visible without changing layout: almost-black navigation against graphite reading surfaces, cyan monospace section headings and luminous cyan selection. Light mode pairs cool white with deep cyan. The cyan signature is independent of a saved Obsidian accent, so custom link/action colors remain intact. `--nd-signal-h` controls its hue; solid-surface and no-glow options still apply.

Controls retain a quieter macOS-like appearance: selection fills without accent borders, compact 4px-radius tags, monospace callout titles and tabular monospace dates/numbers. Buttons keep subtle shadows and keyboard-only focus rings. Inline properties retain their native, borderless editing layout.

The technical-notebook direction pairs a bold 2em monospace note title with smaller H1/H2 section headings and sans-serif prose. In dark mode the reading plane is visibly lighter than the navigation rail. Links and actions default to cyan with calibrated light-mode shades. Custom accent choices remain intact. After hot-swapping theme CSS, Obsidian's virtual file tree may need its layout refreshed to discard cached inline indentation.

Syntax colors are independent of the UI accent: violet keywords, green strings, amber numbers, cyan functions and blue types. Each has a separate light-mode shade, so the light theme is not an inversion of the dark one. Inline code uses a restrained blue tint rather than the link accent.

Bases tables keep their native sizing and editing behavior, with horizontal separators, quiet headers and neutral file links that reveal the accent on hover. Dates and numbers remain tabular; numeric editors align to the end. The Graph control panel uses a neutral elevated surface rather than a permanent accent border. Selection and keyboard focus remain visible in both modes.

Floating menus, suggestions, popovers and Graph controls use smoked glass in dark mode and more opaque frosted glass in light mode. Modals are nearly opaque for readability. Neon stays in active states: a short glow on primary-button hover/keyboard focus and a soft inset light on the selected file. Note text, properties and Bases remain opaque. Unsupported blur and reduced-transparency preferences retain solid surfaces. Style Settings provides **Solid floating surfaces** and **Disable active glow** switches.

Version 1.1.0 applies principles from *Refactoring UI*, its *Color Palettes*, *Component Gallery* and *Font Recommendations* to the existing Neon Dreams theme. It is an adaptation for Obsidian, not a copy of the gallery or an official Refactoring UI theme.

- **Hierarchy before decoration.** Neutral note titles, cyan section headings, distinct weights and generous section spacing keep attention on the note. The workspace grid is opt-in.
- **Readable supporting content.** Labels, placeholders, table headers and code comments use stronger contrast. Primary buttons use a darker fill than inline links to support white text.
- **Deliberate spacing.** A bounded 4/8/12/16/24/32px scale groups related controls and separates sections. Body line height is 1.65, while headings use tighter line heights.
- **Less visual framing.** Tables use horizontal separators, sentence-case sans-serif headers and tabular figures. Code blocks and blockquotes no longer carry decorative indigo borders.
- **Meaningful depth.** Menus, suggestions and dialogs have elevation shadows; everyday content stays flat.
- **Two complete modes.** Light mode uses darker semantic colors rather than putting dark-mode neon on white. Keyboard focus and reduced-motion preferences are respected.

Inter/system sans-serif remains the reading and interface stack. JetBrains Mono defines note titles, H1/H2 headings, code, tags and structured dates/numbers; text-heavy metadata and tables stay sans-serif. Existing user font preferences still take precedence through Obsidian's native font variables.

Please note that I built this theme mostly for myself, so it may not fit every use case.

### If you like the theme

It is completely free, but if you want to throw a few coins in the hat, here is a link.<br><br>
<a href="https://www.buymeacoffee.com/guilhermetagliati" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;"></a>

## Screenshots

These screenshots predate 1.2.0 and do not yet show the night-terminal identity or glass surfaces.

| Dark                                   | Light                                    |
| -------------------------------------- | ---------------------------------------- |
| ![Dark editor](assets/dark-editor.png) | ![Light editor](assets/light-editor.png) |
| ![Dark graph](assets/dark-graph.png)   | ![Light graph](assets/light-graph.png)   |

## Main Features

1. **HSL token system.** Change `--base-h` (background hue) and `--accent-h` (interactive accent hue) to adjust the neutral and accent scales. Text and semantic colors are calibrated separately. Contrast checks apply to the defaults, not every possible custom hue.
2. **Dark and light variants.** A near-black blue dark theme plus a light variant calculated from the same tokens.
3. **Style Settings integration.** Tweak colors and toggle behaviors without editing CSS (requires the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin).
4. **Semantic callouts.** Borderless surfaces with colored icons and titles: cyan for info, green for success, amber for warning, red for danger, muted for quotes. Todo and example have their own accent colors. An outlined variant remains available.
5. **Task states.** Each `data-task` value gets a distinct checkbox icon and color, natively (no plugin required): `[ ]` todo, `[/]` in progress, `[>]` forwarded, `[?]` question, `[x]` done, `[-]` cancelled.
6. **Compact tags.** Tags use monospace text, an accent tint and 4px corners. A plain text variant is available.
7. **Typography.** Sans-serif prose, metadata and tables; monospace note titles, H1/H2, code, tags and structured dates/numbers. Heading size, weight, style and variant tokens remain configurable.
8. **Quiet code blocks.** Recessed background, dedicated light/dark syntax palettes and readable comments, with tinted inline code. Horizontal scroll is available.
9. **Readable tables.** Sans-serif headers, horizontal separators and tabular figures. Full-width and wide layouts are available; wide tables expand only on desktop in Reading view.
10. **Graph view and Canvas.** Nodes, tags, attachments and unresolved links follow the semantic palette. Canvas cards, edges and focus states use the accent.

## Additional Features

1. Optional grid overlay on the workspace (off by default).
2. Five-level text hierarchy that stays readable in grayscale.
3. Configurable readable line width, defaulting to `38rem`; enable Obsidian's Readable line length setting to use it.
4. Active line highlight (opt-in).
5. Hide markdown syntax in Live Preview (opt-in).
6. Minimal status bar and auto-hiding ribbon (opt-in).
7. Disable or speed up animations.

---

#### How to use the Style Settings plugin

1. Install the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin, then enable it.
2. Go to Settings, then open the "Style Settings" tab.

From there you can:

- Set the base hue and saturation (background temperature).
- Set the accent hue and saturation (primary interactive color).
- Set the signature hue for section headings and active navigation independently.
- Set readable line width (`28rem` to `48rem`).
- Enable the optional workspace grid.
- Switch floating surfaces to solid or disable active glow.
- Enable/disable the active line highlight.
- Hide markdown syntax in Live Preview.
- Show/hide editor line numbers.
- Make code blocks scroll horizontally instead of wrapping.
- Hide the ribbon (show on hover).
- Use a minimal status bar (show on hover).
- Disable or speed up all animations.
- Use square checkboxes.
- Render tags as plain text.
- Use outlined, border-only callouts.
- Strip embed borders and titles.
- Use full-width or wide tables.

The line-number toggle styles the editor gutter; enable line numbers in Obsidian's Editor settings as well. CSS cannot create a gutter that the editor has not mounted.

---

## Recommended plugins

1. <a href="https://github.com/mgmeyers/obsidian-style-settings">Style Settings</a> (required for the visual controls above).

## Changelog

See [CHANGELOG.md](CHANGELOG.md).
