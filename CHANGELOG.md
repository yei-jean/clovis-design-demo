# Changelog

All notable changes to this project will be documented in this file.

## 2026-03-31

**Add:**

- **Blog Cover Maker** (`clovis-blog-cover-maker/`): 1200×675 (blog) and 1200×480 (social) covers; title, tint, typography, logo toggle; copy or export PNG (html2canvas, 1×–3× DPR)
- Shared assets under `image/`: `clovis-Logo.svg`, `BlogCover-Background.svg` (loaded via `fetch`; use a local HTTP server, not `file://`)
- Home icon in the toolbar (before the tool title) on Graphic Maker and Blog Cover Maker, linking to the project root index

**Change:**

- Index page: add Blog Cover Maker card alongside Graphic Maker
- Blog Cover Maker: logo and title use the same horizontal inset (60px at 1200px width); logo top offset 64.62px at 675px canvas height (scaled for other heights)

**Fixed:**

- Blog Cover Maker: text color swatch active state when picking presets vs custom color
- Blog Cover Maker: PNG export waits for logo image `decode()` so the mark is not missing on first export

---

## 2026-03-14

**Add:**

- Index page at project root with link to Graphic Maker
- Export scale selector (1×, 1.5×, 2×, 3×) for PNG resolution
- Collapsible editor panel with icon toggle
- Title layout option: same line (inline) or new line (block)
- Editable table headers for Rate Data Table template
- Gradient text export: inline SVG for reliable PNG output across browsers
- Content area color update: blue accent from design tokens

**Change:**

- Rate Data graphic: column spacing adjusted for even distribution

**Fixed:**

- Export PNG gradient text displacement (template-specific vertical nudge)
- Export PNG gradient text wrap/layout when title is long
- Export PNG fallback (html2canvas + SVG foreignObject) for browser compatibility

---

## Format

Entries are grouped by **date** (ISO `YYYY-MM-DD`). Under each date:

- **Add** — New features
- **Change** — Changes in existing functionality
- **Fixed** — Bug fixes
