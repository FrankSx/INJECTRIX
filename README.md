# INJECTRIX

**A self-contained browser-console JS arsenal for web-app recon, injection
testing, and reporting — with a headless Playwright driver for automation.**

No build step. No server. No dependencies for the arsenal itself. Open one
HTML file and work.

![snippets](https://img.shields.io/badge/snippets-67-4af0c0) ![categories](https://img.shields.io/badge/categories-12-4a9df0) ![templates](https://img.shields.io/badge/mission%20templates-8-f0b44a) ![license](https://img.shields.io/badge/license-MIT-green)

## What's inside

| Path | What it is |
|---|---|
| `arsenal/INJECTRIX.html` | The console tool — 67 snippets across 12 categories, 8 mission templates, mission builder, dual-mode copy, full report engine |
| `driver/irx_driver.js` | Playwright headless bridge — walks a target list, injects bootstrap + template per target, harvests `__IRX` reports, writes per-target JSON + `AGGREGATE.md` |
| `driver/targets.txt` | Target list for the driver (one per line, `#` comments) |
| `CATALOG.md` | Full snippet index, generated from the live HTML |

## Categories

Recon · Traffic Hooks · Auth & Tokens · DOM Analysis · Injection Testing ·
Framework · Egress · Utility · Advanced · Automation · mXSS · Report

## Quick start (console)

1. Open `arsenal/INJECTRIX.html` in any browser.
2. Load a **mission template** (or queue snippets manually).
3. Paste the chained payload into the target page's console.
4. In the target: `__IRX.export()` → paste into the **REPORT** tab → annotate
   severities/notes → export Markdown, standalone HTML, or JSON.

Every snippet also has a **copy + capture** mode that auto-logs its result
(sync, async, and errors) into the in-page report engine.

## Quick start (headless)

```bash
npm i playwright && npx playwright install chromium
node driver/irx_driver.js driver/targets.txt "Full Recon Sweep" [stepDelayMs]
```

Templates: `Full Recon Sweep` · `XSS / mXSS Hunt (post-flood)` ·
`XSS Hunt - phase 1` · `Auth Audit` · `XS-Leak Kit` · `API Surface Map` ·
`PP + Clobber` · `Automation Recon`

## The report engine

The IRX bootstrap (`zz-irx-bootstrap` snippet) installs `window.__IRX` in the
target page:

```js
__IRX.log(title, data, severity)   // capture a finding
__IRX.note(title, text)            // analyst note
__IRX.md() / __IRX.html()          // render report
__IRX.copy() / __IRX.copyHtml()    // copy to clipboard
__IRX.export()                     // JSON for the REPORT tab
__IRX.count() / __IRX.clear()      // helpers
```

## Contributing

Additions welcome: new snippets (see `CATALOG.md` for conventions), new
mission templates, driver improvements. Keep snippets dependency-free and
parse-valid — every snippet is syntax-checked against the catalog.

## Legal

See [SECURITY.md](SECURITY.md). Authorized testing only.
