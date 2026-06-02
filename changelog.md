# Apogee Essential Edition — HTML Revision Summary

**File:** `apogee-essential-edition.html`  
**Revised file:** `apogee-essential-edition-v2.html`  
**Date:** 2 June 2026  
**Revised by:** OpenCode

---

## Overview

A review of `apogee-essential-edition.html` was carried out covering HTML structure, SEO metadata, Schema.org structured data, accessibility, CSS, and content accuracy. The file was found to be well-formed overall. One cross-browser rendering bug was identified and corrected in the revised version.

---

## Change Made

### Fix: WebKit disclosure triangle on FAQ `<summary>` elements

| | |
|---|---|
| **Location** | CSS block — `summary` rule (line 381–391) |
| **Type** | Bug fix |
| **Browsers affected** | Google Chrome, Microsoft Edge, Safari |

**Problem**

The FAQ accordion uses `<details>` / `<summary>` elements with a custom `+` / `−` toggle indicator. The original CSS used `list-style: none` on `<summary>` to suppress the default disclosure arrow. This works in Firefox but does **not** remove the native WebKit disclosure triangle in Chrome, Edge, and Safari — causing both the native arrow and the custom `+` symbol to appear side by side.

**Fix applied**

Added the vendor-prefixed pseudo-element rule to explicitly hide the WebKit marker:

```css
/* Original (v1) */
summary {
  list-style: none;
  /* ... */
}
summary::after { content: '+'; font-size: 1.2rem; color: #0057a8; }

/* Revised (v2) */
summary {
  list-style: none;
  /* ... */
}
summary::-webkit-details-marker { display: none; }
summary::after { content: '+'; font-size: 1.2rem; color: #0057a8; }
```

**Result:** The custom `+` / `−` indicator now renders correctly as the sole toggle marker in all major browsers.

---

## Items Reviewed — No Changes Required

| Area | Verdict |
|---|---|
| HTML5 document structure | Pass |
| `<meta charset>`, `<meta viewport>` | Pass |
| SEO title, description, keywords | Pass |
| Canonical URL | Pass |
| Open Graph tags (og:type, og:title, og:description, og:image) | Pass |
| Twitter Card tags | Pass |
| Schema.org — `SoftwareApplication` block | Pass |
| Schema.org — `BreadcrumbList` block | Pass |
| Schema.org — `FAQPage` block | Pass |
| ARIA attributes (`aria-labelledby`, `aria-label`, `aria-hidden`, `aria-current`) | Pass |
| Responsive CSS (`clamp()`, `auto-fit` grid, media query) | Pass |
| Comparison table content | Pass |
| System requirements content | Pass |
| FAQ content consistency with structured data | Pass |
| Footer copyright year (2026) | Pass |

---

## File Reference

| File | Description |
|---|---|
| `apogee-essential-edition.html` | Original — unchanged |
| `apogee-essential-edition-v2.html` | Revised — WebKit disclosure marker fix applied |
| `changelog.md` | This document |
| `changelog.pdf` | PDF version of this document |
