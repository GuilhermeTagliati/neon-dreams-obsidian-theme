# Changelog

All notable changes to Neon Dreams are documented here.

## 1.1.0 (2026-10-25)

### Changed

- Refine Neon Dreams using the supplied Refactoring UI book, color palettes, component gallery and font recommendations while retaining indigo accents and semantic task states
- Use less-saturated charcoal surfaces with clearer separation between the editor, sidebars and elevated overlays
- Replace colored section headings with a neutral 30/24/20/18/16/14-equivalent type scale, proportional heading line heights and larger section spacing
- Set default readable line width to `38rem` and body line height to 1.65
- Increase supporting-text contrast, including table headers, metadata labels, placeholders and code comments
- Separate primary-button fills from brighter link colors for legible white button text
- Use sans-serif metadata and tables with tabular figures; reserve monospace for code and tags
- Replace full table grids with horizontal separators and remove decorative accent borders from code blocks and blockquotes
- Add elevation shadows to menus, suggestions and dialogs; make the workspace grid opt-in
- Complete light-mode native-variable mappings and darken its semantic colors and callout titles
- Restrict general input styling to text-like controls so it does not restyle toggles, checkboxes, ranges or color pickers

### Added

- Style Settings controls for readable line width and workspace grid
- Visible keyboard focus and system reduced-motion support
- Compact callout/code padding on narrow screens and keyboard-accessible reveal for auto-hidden ribbon/status bar

### Fixed

- Match body-level active-line, square-checkbox and plain-tag feature flags correctly
- Reserve the explorer selection border on inactive files to avoid shifting labels
- Keep wide tables inside their scroll wrapper on mobile; desktop widening is limited to Reading view
- Restore a visible outline for the outlined-callout option after simplifying default callout borders

### Notes

- Existing screenshots predate this release. Contrast verification covers the default palette, not arbitrary user-selected colors.

## 1.0.2 (2026-06-27)

### Fixes

- Drop multi-value `text-decoration` shorthand (e.g. `line-through <color>`) in favor of the single-keyword form for full compatibility
- Bump `minAppVersion` from `1.1.0` to `1.6.0`

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
