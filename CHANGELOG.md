# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Added

- **Blog Cover Maker** (`clovis-blog-cover-maker/`): 1200×675 (blog) and 1200×480 (social) covers; title, tint, typography, logo toggle; copy or export PNG (html2canvas, 1×–3× DPR)
- Shared assets under `image/`: `clovis-Logo.svg`, `BlogCover-Background.svg` (loaded via `fetch`; use a local HTTP server, not `file://`)
- Index page at project root with links to Graphic Maker and Blog Cover Maker
- Export scale selector (1x, 1.5x, 2x, 3x) for PNG resolution
- Collapsible editor panel with icon toggle
- Title layout option: same line (inline) or new line (block)
- Editable table headers for Rate Data Table template
- Gradient text export fix: inline SVG for reliable PNG output across browsers
- Content area color update: blue accent from design tokens

### Changed

- Rate Data graphic: column spacing adjusted for even distribution
- Blog Cover Maker: logo and title use the same horizontal inset (60px at 1200px width); logo top offset 64.62px at 675px canvas height (scaled for other heights)

### Fixed

- Export PNG gradient text displacement (template-specific vertical nudge)
- Export PNG gradient text wrap/layout when title is long
- Export PNG fallback (html2canvas + SVG foreignObject) for browser compatibility
- Blog Cover Maker: text color swatch active state when picking presets vs custom color
- Blog Cover Maker: PNG export waits for logo image `decode()` so the mark is not missing on first export

---

## Format

- **Added** – New features
- **Changed** – Changes in existing functionality
- **Fixed** – Bug fixes
- **Removed** – Removed features
