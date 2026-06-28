# Changelog

All notable changes to Neon Dreams are documented here.

## 1.0.1 (2026-06-27)

### Fixes

- Remove non-standard `scrollbar-color` / `scrollbar-width` (webkit pseudo-elements already cover Electron)
- Replace `text-decoration-line` / `text-decoration-color` longhands with the `text-decoration` shorthand for broader compatibility
- Remove all `!important` overrides in favor of higher selector specificity (`body` prefix) and Obsidian CSS variables (`--checkbox-color`, `--checkbox-marker-color`)

## 1.0.0 (2026-06-27)

Initial release. A dark Obsidian theme with a precise, structured aesthetic.

### Colors

- HSL token system: change `--base-h` and `--accent-h` to retheme the entire interface
- Layered blue-black background scale derived from a single base hue and saturation
- Indigo primary accent for links, focus, active states and interactive elements
- Fixed semantic colors: green for success, red for danger, cyan for data and info, amber for warnings
- Five-level text hierarchy that stays readable in grayscale
- Light variant with an HSL palette calculated from the same base and accent hues

### Typography and layout

- Configurable heading scale through `--h1` to `--h6` size, weight, style and variant tokens
- Readable line width (`42rem`) with independent container widths for tables and images
- Sans-serif (Inter) for prose, JetBrains Mono for code, data, metadata and tables
- Terminal-style code blocks with an accent left border, plus inline code styling

### Components

- Callouts with semantic left-border accents (info, success, warning, danger, quote)
- Task states per `data-task`: distinct checkbox icon and color, plus title styling
- Tag pills with an indigo tint
- Table headers in an uppercase monospace label style
- Graph view and Canvas styled to match the palette
- Subtle grid overlay on the workspace

### Style Settings

Optional integration with the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin, exposing visual controls without editing CSS:

- Color controls: base hue and saturation, accent hue and saturation
- Editor toggles: active line highlight, hide markdown syntax, line numbers, horizontal code scroll
- Interface toggles: hide ribbon, minimal status bar, disable or speed up animations
- Content toggles: square checkboxes, plain text tags, outlined callouts, strip embed decorations
- Table toggles: full-width and wide tables
