# HubSpot CMS Clean Starter Theme

A zero-bloat, production-ready HubSpot CMS starter theme built with clean semantic **HubL** and scoped CSS. Designed to score **95+ on mobile Google Lighthouse** and run 100% on **HubSpot Content Hub Starter ($20/month)** without marketplace theme bloat or jQuery dependencies.

Maintained by **[Native Rebuild](https://nativerebuild.com)** — Fixed-Price HubSpot Website Migration & Custom HubL Development.

---

## Why This Starter Exists

Most HubSpot Marketplace themes bundle 400–600 KB of unused CSS, legacy jQuery, and third-party carousel libraries across every page, dragging mobile Core Web Vitals down into the 40–65 range.

This starter gives B2B engineering and marketing teams a clean foundation:
- **Zero jQuery or external JS frameworks**
- **Works on Content Hub Starter ($20/mo)** — no Professional or Enterprise tier required
- **Strict drag-and-drop (`dnd_area`) support** for non-technical marketers
- **Scoped CSS custom properties** for easy brand token configuration
- **Clean semantic HTML5** for SEO and accessibility

---

## Included Structure

```text
hubspot-cms-clean-starter/
├── theme.json
├── css/
│   └── main.css
├── templates/
│   ├── layouts/
│   │   └── base.html
│   └── landing-page.html
└── modules/
    ├── hero-section.module/
    │   ├── meta.json
    │   ├── fields.json
    │   └── module.html
    └── feature-grid.module/
        ├── meta.json
        ├── fields.json
        └── module.html
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
4. Create a new page in HubSpot (`Marketing > Website > Website Pages`) and select the **Landing Page** template under `hubspot-cms-clean-starter`.

---

## Helpful HubSpot Migration & Architecture Guides

If you are migrating an existing design or website into HubSpot CMS, check out our technical resources:
- [HubSpot Website Migration Service](https://nativerebuild.com/hubspot-website-migration)
- [2026 HubSpot Website Migration Cost Guide](https://nativerebuild.com/hubspot-website-migration-cost)
- [HubSpot Content Hub Tiers Guide: Starter vs. Pro vs. Enterprise](https://nativerebuild.com/hubspot-content-hub-tiers-guide)
- [32-Point HubSpot SEO Migration Checklist](https://nativerebuild.com/hubspot-migration-seo-checklist)
- [HubSpot Marketplace Themes vs. Custom Rebuild](https://nativerebuild.com/hubspot-marketplace-themes-vs-custom-rebuild)

---

## License

MIT License — free to use for commercial and personal HubSpot CMS projects.
