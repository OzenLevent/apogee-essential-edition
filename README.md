# Apogee Essential Edition — Product Page Repository

## Purpose

This repository tracks the development and revision history of the **Apogee Essential Edition** product page for [eco3.com](https://eco3.com).

The page is being created using AI-assisted documentation tools as part of a structured content workflow. It will be published to `https://eco3.com/products/apogee-essential-edition` following SME review and sign-off.

---

## Background

Apogee Essential Edition is a new ECO3 product based on the existing Apogee prepress workflow architecture, scoped for small commercial printers with fewer than 10 employees and an annual plate volume of up to 2,500 m². No product page currently existed on eco3.com.

An initial draft was produced using AI-assisted documentation, leveraging existing Apogee product information as a reference. The draft is undergoing SME validation before publishing.

---

## Repository Contents

| File | Description |
|---|---|
| `apogee-essential-edition.html` | Original AI-generated product page draft |
| `apogee-essential-edition-v2.html` | Revised version — cross-browser FAQ rendering fix applied |
| `changelog.md` | Summary of changes between versions |

> Non-HTML files (PDF, TXT, exports) are kept locally and excluded from this repository via `.gitignore`.

---

## Page Structure

The HTML product page includes:

- Full SEO metadata (title, description, keywords, canonical URL)
- Open Graph and Twitter Card tags
- Schema.org structured data: `SoftwareApplication`, `BreadcrumbList`, `FAQPage`
- Product overview and target audience
- Key features grid
- Comparison table (Essential Edition vs. full Apogee)
- System requirements
- FAQ section
- Related products
- CTA section

---

## Workflow

```
AI draft → HTML review → revision → SME review → corrections → publish to eco3.com
```

### Status

| Deliverable | Status |
|---|---|
| Product page draft (HTML) | Done — pending SME review |
| Schema.org structured data | Done — pending SME review |
| HTML revision (v2) | Done |
| SME-reviewed and corrected page | Pending |
| Published page on eco3.com | Pending |
| URL submitted to search engines | Pending |

---

## SME Review Required

Before publishing, the following must be validated:

| Area | Reviewer Role |
|---|---|
| Product capabilities and features | Apogee Product Manager |
| Technical specifications | Engineering / Pre-sales |
| Plate volume threshold (2,500 m²/year) | Sales / Product Marketing |
| Licensing model | Sales / Legal |
| Market positioning and messaging | Product Marketing |
| Legal and branding compliance | Marketing / Legal |

---

## Acceptance Criteria

- [ ] All SME review comments addressed and signed off
- [ ] Page passes [Google Rich Results Test](https://search.google.com/test/rich-results) with no errors
- [ ] Valid `SoftwareApplication`, `BreadcrumbList`, and `FAQPage` schemas confirmed
- [ ] Page is live at `https://eco3.com/products/apogee-essential-edition`
- [ ] Page is linked from the ECO3 products listing page
- [ ] URL submitted to Google Search Console
- [ ] URL submitted to Bing Webmaster Tools
- [ ] Page loads in under 3 seconds (Core Web Vitals baseline)

---

## References

| Item | Location |
|---|---|
| Existing Apogee product page | https://eco3.com/products/apogee |
| ECO3 products listing | https://eco3.com/products |
| Google Rich Results Test | https://search.google.com/test/rich-results |
| Google Search Console | https://search.google.com/search-console |
| Bing Webmaster Tools | https://www.bing.com/webmasters |
| Jira ticket | `[DOC] Apogee Essential Edition – AI-assisted product page creation, SEO & SME review` |

---

## Labels

`documentation` `seo` `ai-assisted` `apogee` `product-page` `sme-review`
