# Jira Ticket: [DOC] Apogee Essential Edition – AI-assisted product page creation, SEO & SME review

---

## Summary
Create a publicly accessible, SEO-optimized product page for **Apogee Essential Edition** using AI-assisted documentation tools. The page must be discoverable by search engines and AI-powered search tools (Google AI Overviews, Bing Copilot, Perplexity), and must be validated by Subject Matter Experts before publishing.

---

## Background
Apogee Essential Edition is a new product based on the existing Apogee prepress workflow architecture, scoped and optimized for small commercial printers with fewer than 10 employees and an annual plate volume of up to 2,500 m². No product page currently exists on eco3.com.

An initial draft of the product page has been produced using AI-assisted documentation, leveraging the existing Apogee product information on eco3.com as a reference. The draft requires SME validation before it can be published.

---

## Objectives
- Produce a complete, publish-ready HTML product page for Apogee Essential Edition
- Ensure the page is discoverable via internet search engines and AI-powered search tools
- Embed structured metadata (Schema.org, Open Graph) for maximum search visibility
- Obtain SME sign-off on all product claims, specifications, and positioning before publishing

---

## Scope

### In scope
- HTML product page with full SEO metadata
- Schema.org structured data (SoftwareApplication, BreadcrumbList, FAQPage)
- Open Graph and Twitter Card tags
- Product description, feature list, system requirements, comparison table, FAQ section
- SME review and correction cycle
- Publishing to eco3.com under `/products/apogee-essential-edition`
- Submission of URL to Google Search Console and Bing Webmaster Tools

### Out of scope
- Apogee Essential Edition software development
- Translation into languages other than English (separate ticket)
- Paid search / advertising campaigns

---

## Deliverables
| # | Deliverable | Format | Status |
|---|---|---|---|
| 1 | Product page draft | HTML | Done – pending SME review |
| 2 | Schema.org structured data | JSON-LD embedded in HTML | Done – pending SME review |
| 3 | Chat session & methodology export | MD + PDF | Done |
| 4 | SME-reviewed and corrected page | HTML | Pending |
| 5 | Published product page | Live URL on eco3.com | Pending |
| 6 | URL submitted to search engines | Google Search Console + Bing | Pending |

---

## SME Review Required

The following areas must be validated by the relevant Subject Matter Experts before publishing:

| Area | Reviewer Role | Items to Validate |
|---|---|---|
| Product capabilities | Apogee Product Manager | Feature list, module names, capability boundaries vs. full Apogee |
| Technical specifications | Engineering / Pre-sales | OS support, RAM, storage, APPE version, CtP compatibility |
| Plate volume threshold | Sales / Product Marketing | Confirm 2,500 m²/year as the correct Essential Edition boundary |
| Licensing model | Sales / Legal | License terms, pricing description, what is included |
| Market positioning | Product Marketing | Target audience definition, messaging, competitor differentiation |
| Legal / branding | Marketing / Legal | ECO3 brand guidelines, trademark usage, required disclaimers |

---

## Acceptance Criteria
- [ ] All SME review comments have been addressed and signed off
- [ ] Page passes validation at https://search.google.com/test/rich-results (no errors)
- [ ] Page contains valid SoftwareApplication, BreadcrumbList, and FAQPage schemas
- [ ] Page is live at `https://eco3.com/products/apogee-essential-edition`
- [ ] Canonical URL is correctly set in the HTML `<head>`
- [ ] Page is linked from the main ECO3 products listing page
- [ ] URL has been submitted to Google Search Console
- [ ] URL has been submitted to Bing Webmaster Tools
- [ ] Page loads in under 3 seconds (Core Web Vitals baseline)

---

## Subtasks
1. `[DOC-01]` SME review of product capabilities and feature list
2. `[DOC-02]` SME review of technical specifications
3. `[DOC-03]` SME review of licensing model and pricing description
4. `[DOC-04]` Legal / branding sign-off
5. `[DOC-05]` Apply SME corrections to HTML page
6. `[DOC-06]` Validate structured data (rich results test)
7. `[DOC-07]` Publish page to eco3.com CMS
8. `[DOC-08]` Submit URL to Google Search Console and Bing Webmaster Tools
9. `[DOC-09]` Verify page appears in search results (2–4 weeks post-publish)

---

## References
| Item | Location |
|---|---|
| Draft HTML product page | `Apogee_Essentials_Edition\apogee-essential-edition.html` |
| Chat session export (MD) | `Apogee_Essentials_Edition\chat-export.md` |
| Chat session export (PDF) | `Apogee_Essentials_Edition\chat-export.pdf` |
| Existing Apogee product page | https://eco3.com/products/apogee |
| ECO3 products listing | https://eco3.com/products |
| Google Rich Results Test | https://search.google.com/test/rich-results |
| Google Search Console | https://search.google.com/search-console |
| Bing Webmaster Tools | https://www.bing.com/webmasters |

---

## Priority
**Medium** — product is in development; page should be ready to publish at product launch.

## Labels
`documentation` `seo` `ai-assisted` `apogee` `product-page` `sme-review`
