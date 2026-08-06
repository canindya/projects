# Changelog

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
