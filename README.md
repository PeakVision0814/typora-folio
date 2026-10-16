# Folio · 纸间

A modern editorial theme for Typora, with warm colors, serif body text, and a quiet reading rhythm.

**English** · [简体中文](README.zh-CN.md)

## Preview

### Folio — light

Warm paper tones with moss-green accents.

![Folio light theme with bilingual text, headings, a quote, and lists](docs/images/folio.png)

### Folio Night — dark

Warm charcoal with sage-green accents.

![Folio Night dark theme with bilingual text, headings, a quote, and lists](docs/images/folio-night.png)

These screenshots are rendered from the included [browser preview](folio/preview.html). The sidebar illustrates theme colors; actual Typora controls and rendering may differ. Open the preview locally to switch between both palettes.

## Features

- Two palettes sharing the same typography and layout.
- Bundled STIX Two Text for Latin text, with local Chinese serif font fallbacks.
- Sans-serif headings, 17px body text, and 1.8 line spacing.
- A reading area that uses 90% of the editor width and adapts to narrow windows.
- Coordinated styles for tables, quotes, code, task lists, and footnotes.
- A white background with dark text for printing and PDF export.

## Installation

1. Download this repository using **Code → Download ZIP**, then extract it.
2. In Typora, open **Preferences → Appearance → Open Theme Folder**.
3. Copy `folio.css`, `folio-night.css`, and the entire `folio` folder into that theme folder. Keep their relative paths intact.
4. Restart Typora and select **Folio** or **Folio Night** from the **Themes** menu.

Your theme folder should contain:

```text
themes/
├── folio.css
├── folio-night.css
└── folio/
    ├── folio-base.css
    ├── STIX2Text-Regular.woff
    ├── STIX2Text-Italic.woff
    ├── STIX2Text-Bold.woff
    ├── STIX2Text-BoldItalic.woff
    └── STIX_2.0.0_license.pdf
```

The `docs` folder and root README files are only needed for the repository documentation.

## Fonts and customization

STIX Two Text is included. Chinese body text prefers Source Han Serif / Noto Serif CJK SC / Noto Serif SC, falling back to Songti SC or SimSun. Headings use available system sans-serif fonts. Code uses Cascadia Code, JetBrains Mono, or Consolas when available. Fonts are loaded locally.

Edit `folio.css` or `folio-night.css` to change colors. Shared typography and layout live in `folio/folio-base.css`:

```css
:root {
    --folio-body-size: 17px;
    --folio-line-height: 1.8;
    --folio-reading-width: 90%;
}
```

After editing, copy the changed files into Typora's theme folder and reselect the theme. See [theme notes](folio/README.md) for more details.

## Font license

The bundled STIX fonts retain their accompanying [license](folio/STIX_2.0.0_license.pdf).
