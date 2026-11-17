# HubSpot CMS Clean Starter Theme

A zero-bloat, production-ready HubSpot CMS starter theme built with clean semantic **HubL**, global theme settings (`fields.json`), automatic **SEO / AEO JSON-LD schema**, and scoped CSS. Designed to score **95–100 on mobile Google Lighthouse** and run 100% on **HubSpot Content Hub Starter ($20/month)**.

Maintained by **[Native Rebuild](https://nativerebuild.com)** — Fixed-Price HubSpot Website Migration & Custom HubL Development.

---

## What Makes This Starter Different?

Most HubSpot Marketplace themes and boilerplates ship 400–600 KB of unused CSS, legacy jQuery, and third-party JavaScript libraries across every page—dragging mobile Core Web Vitals into the 40–65 range.

This starter gives B2B engineering and marketing teams capabilities other free starters skip:

| Capability | Typical HubSpot Starter / Marketplace Theme | `hubspot-cms-clean-starter` |
| :--- | :--- | :--- |
| **JavaScript Overhead** | jQuery + Slick/AOS/Lightbox bundles (300 KB+) | **0 KB external JS** (Zero-JS `<details>` accordions & mobile drawer) |
| **Automatic SEO & AEO Schema** | Manual JSON-LD pastes in page settings | **Built-in `Organization`, `WebPage`, `BlogPosting`, and `FAQPage` JSON-LD** |
| **Native HubSpot Form Styling** | Unstyled forms or slow iframe overrides | **Pre-styled `.nr-form-card`** with zero layout shift (CLS = 0) |
| **Theme Token Controls** | Complex nested overrides | **Clean `fields.json` → CSS Custom Properties** (`theme-overrides.css`) |
| **HubSpot Tier Required** | Often relies on Pro/Enterprise features | **100% Content Hub Starter ($20/mo)** compatible |

---

## Included Architecture

```text
hubspot-cms-clean-starter/
├── theme.json                         # HubSpot theme manifest
├── fields.json                        # Global Brand Colors, Layout & Schema settings
├── css/
│   ├── main.css                       # Scoped layout, header, form, and accordion CSS
│   └── theme-overrides.css            # HubL bridge mapping fields.json to CSS variables
├── templates/
│   ├── layouts/base.html              # Semantic HTML5 shell + automatic SEO schema
│   ├── partials/
│   │   ├── header.html                # Sticky header + zero-JS mobile menu drawer
│   │   ├── footer.html                # Responsive footer
│   │   └── seo-schema.html            # Automatic Organization & WebPage JSON-LD
│   ├── home.html                      # Full B2B Home Page template (dnd_area)
│   ├── landing-page.html              # Conversion-focused Landing Page template
│   ├── blog-index.html                # 3-column responsive Blog Listing + pagination
│   ├── blog-post.html                 # Readable Blog Post + automatic BlogPosting schema
│   └── system/404.html                # Branded 404 Error Page
└── modules/
    ├── hero-section.module/           # Hero with eyebrow, H1, subheadline, and CTA
    ├── social-proof.module/           # Lazy-loaded B2B logo trust bar
    ├── feature-grid.module/           # Configurable 1–6 card CSS Grid
    ├── faq-accordion.module/          # Zero-JS <details> FAQ + auto FAQPage JSON-LD
    └── native-form-cta.module/        # Split CTA section with styled native HubSpot Form
```

---

## Quick Start (HubSpot CLI)

1. Install the HubSpot CLI and authenticate with your portal:
   ```bash
   npm install -g @hubspot/cli
   hs init
   ```
2. Clone this repository:
   ```bash
   git clone https://github.com/nativerebuild/hubspot-cms-clean-starter.git
   cd hubspot-cms-clean-starter
   ```
3. Upload the theme to your HubSpot Design Manager:
   ```bash
   hs upload . hubspot-cms-clean-starter
   ```
4. Create a page in HubSpot (`Marketing > Website > Website Pages`) and select **Home Page** or **Clean Landing Page** under `hubspot-cms-clean-starter`.

---

## HubSpot Migration & Architecture Resources

Migrating an existing website or design system into HubSpot CMS? Explore our open engineering guides:
- [HubSpot Website Migration Service](https://nativerebuild.com/hubspot-website-migration)
- [2026 HubSpot Website Migration Cost Guide](https://nativerebuild.com/hubspot-website-migration-cost)
- [HubSpot Content Hub Tiers Guide: Starter vs. Pro vs. Enterprise](https://nativerebuild.com/hubspot-content-hub-tiers-guide)
- [32-Point HubSpot SEO Migration Checklist](https://nativerebuild.com/hubspot-migration-seo-checklist)
- [HubSpot Marketplace Themes vs. Custom Rebuild](https://nativerebuild.com/hubspot-marketplace-themes-vs-custom-rebuild)

---

## License

MIT License — free for commercial and personal HubSpot CMS projects.
