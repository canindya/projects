# Changelog

## [2026-09-02]

### Changed
- **Editorial redesign**: Both pages rebuilt as a numbered index — one construction per project (number, serif title, stat line, one paragraph, status/stack line, image frame) on a 12-column grid with 80px margins. Page height down from ~4,470px to ~3,310px
- **Type system**: Cormorant Garamond + DM Sans 300 replaced with Instrument Serif + Instrument Sans; one display size, one title size, three text sizes
- **Palette**: Warm paper `#f3f0e9` and ink `#131211` with a single oxblood accent used only for live status and hover; dark mode is a designed warm charcoal rather than an inversion
- **Screenshots art-directed**: Each source screenshot cropped to one meaningful region (`kolkata-map`, `westbengal-gsdp`, `cost-of-living-map`) and the RemindMe device cut out of its marketing page onto a theme-aware ground
- **StockPicker**: The "no public build yet" placeholder replaced with a typographic table of the six pipeline stages and their figures
- **About page**: Rebuilt on the same system — a hairline record of roles with years, titles and outcomes in three columns
- **West Bengal artefact**: The GSDP-chart-only crop was ~60% empty navy. Replaced with the state overview — headline findings, the trend chart and the summary figure row; `westbengal-gsdp.jpg` renamed to `westbengal-overview.jpg`

### Removed
- **Decorative furniture**: Scroll-progress bar, hide-on-scroll nav, all entrance/reveal animations, the philosophical pull-quote section, the three-up stat strip, the "scroll to explore" affordance, the pill button, and the bordered project cards
- **Italic accent headlines**: The blue italic accent word in "end to *end*", "Selected *works*" and "Finance, Function, *Fiction*"
- **Uppercase monospace micro-labels**: Nine instances reduced to one status/stack line per project

### Fixed
- **Image aspect ratios**: Intrinsic `height` attributes were overriding `aspect-ratio`, so every project frame rendered at its source height instead of one shared 3:2 ratio
- **Copy**: "Tobaco" and "one of top 10 banks" in the TCS entry
- **Off-ratio project crops**: The Cost of Living and West Bengal crops were 1.60 against a 3:2 frame, so `object-fit: cover` trimmed them a second time and cut the cost-of-living colour legend. Both recropped to exactly 3:2, so nothing is cropped in the browser

## [2026-08-07]

### Added
- **Project screenshots**: Captured live screenshots of all four shipped projects into `assets/` — Kolkata ward map, West Bengal state dashboard, Cost of Living explore view, and the RemindMe landing page (16:10, progressive JPEG)
- **Project cards**: Featured project now uses an editorial two-column layout with a screenshot; the other four sit in a 2-up grid with thumbnails and whole-card click targets
- **Featured facts row**: Verifiable figures for the Kolkata dashboard (141 wards, 30+ primary sources, 19 domains)
- **SEO/social**: Meta description, Open Graph and Twitter card tags, `og:image`, theme-color for both schemes, and an inline SVG favicon on both pages
- **Accessibility**: `prefers-reduced-motion` support on both pages

### Fixed
- **Broken project links**: Kolkata and West Bengal dashboards pointed at `canindya.github.io` URLs that returned 404 (private repos, Pages never served). Repointed to `kolkata.datacarta.in` and `westbengal.datacarta.in`
- **Inaccurate project claims**: Corrected against the live products — Kolkata is 19 domains (was 18); Cost of Living covers 180+ countries over 25 years (was 193 countries); added West Bengal's 19 domains / 40+ sources / 23 districts
- **RemindMe**: Removed the unsubstantiated HIPAA tag; description now reflects the shipped product (9 languages, no ads, no paywall, Google Play)
- **Theme flash**: Theme is now set by a blocking script in `<head>` and follows `prefers-color-scheme` when no preference is saved
- **Forced dark mode**: Added `color-scheme` declarations so Chrome's auto dark mode stops inverting the page and flattening status indicators
- **Card thumbnails**: Set `min-height: 0` so flex `min-height: auto` no longer pins images to their intrinsic height
- **Footer**: Copyright year corrected to 2026

### Changed
- **Visual restraint**: Removed the page loader, ambient orbs, cursor glow, noise overlay, card spotlight hover, and fake page-transition fade from both pages
- **Gradients**: Replaced every accent gradient with a solid accent; dropped the now-unused `--accent-2`, `--accent-glow`, `--accent-soft`, `--card-glow` and `--noise-opacity` variables
- **Copy**: Hero rewritten from "Things I build after hours" to a concrete description of the work; removed marketing filler from the hero, writing and footer copy
- **About strip**: Replaced the unverifiable `$150M+` and non-numeric `AI×1` stats with 4 live in production / 15+ years in product / Solo
- **Project detail**: Dropped the per-project "What's Next" and "The Insight" blocks; tags capped at three per project

## [2026-04-17]

### Changed
- **West Bengal Through Data**: Updated status from "Building" to "Live" and added public link to https://canindya.github.io/State-WestBengal/

## [2026-04-13]

### Added
- **West Bengal Through Data**: Added as project 05 — district-level open-data dashboard for West Bengal (Building, no public link)

### Changed
- **Kolkata City Dashboard**: Renamed from "City Kolkata"; updated description and tagline to reflect expanded coverage — now 18 domains, 30+ data sources, 141-ward choropleth, 75-year IMD climate records, 40-year metro ridership series, and cross-domain correlation insights

## [2026-03-31]

### Removed
- **WorldMonitor**: Removed from projects (forked repository, not original work)
- **Projects**: Renumbered City Kolkata from 05 to 04

## [2026-03-29]

### Changed
- **Design**: Major visual overhaul — page loader, scroll progress bar, smart hide/show nav, cursor glow effect, multiple animated ambient orbs, scroll-triggered reveal animations, gradient accents, card spotlight hover effect, smooth page transitions
- **Design**: New color palette — clean neutral backgrounds with deep blue accent (#2563eb/#0ea5e9) replacing warm beige/gold
- **Mobile**: Added hamburger menu with animated toggle and full-screen nav overlay
- **Tags/Buttons**: Pill-shaped tags and CTA buttons for modern feel

### Added
- **WorldMonitor**: Added as project 04 — AI-powered geopolitical intelligence dashboard (Live)
- **City Kolkata**: Added as project 05 — 10-domain open-data dashboard for Kolkata (Live)

## [2026-03-09]

### Changed
- **RemindMe**: Updated project status from "Active Development" to "Live"
