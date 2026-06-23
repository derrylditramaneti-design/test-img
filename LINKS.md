# YoboLabs link registry

> Single source of truth for cross-page links. **Update this file whenever you add, move, or rename a page** so links in the main site and sub-pages stay correct.
> Referenced from code via: `<!-- Links registry: .../LINKS.md -->`

_Last generated from the live blog build: 12 articles._

## Canonical URLs
| Page | URL |
|---|---|
| Home (global) | https://yobolabs.ai |
| Blog index | https://global.pages.yobolabs.ai/blog |
| Get started (CTA) | https://yobolabs.ai/get-started |

**Rule (Derryl):** cross-link the home site as a *bare global* hash — `https://yobolabs.ai/#<id>` — never the `/id/` redirect path.

## Home anchors (link targets on yobolabs.ai)
- `#capabilities` → https://yobolabs.ai/#capabilities
- `#faq` → https://yobolabs.ai/#faq
- `#founders` → https://yobolabs.ai/#founders
- `#how-we-grow` → https://yobolabs.ai/#how-we-grow
- `#success-stories` → https://yobolabs.ai/#success-stories

Other home routes used: `https://yobolabs.ai/get-started`

## Blog articles
Articles are embedded in one microsite (`/blog`) via a hash router. **Until real per-article URLs exist, the only working address is `/blog#<slug>`** (a `/blog/<slug>` path is a 404; the `#` fragment is also why social OG previews can't be per-article — scrapers see the blog index OG).

| Slug | Working URL | Title |
|---|---|---|
| `agency-vs-hire-vs-ai-growth-marketer` | `/blog#agency-vs-hire-vs-ai-growth-marketer` | Email Marketing Agency vs. Full-Time Hire vs. AI Growth Marketer |
| `ai-flows-vs-manual-campaigns` | `/blog#ai-flows-vs-manual-campaigns` | AI Flows vs. Manual Campaigns: Which Drives More Revenue? |
| `beauty-brands-email` | `/blog#beauty-brands-email` | AI Email Marketing for Shopify Beauty Brands: What's Working in 2026 |
| `email-marketing-cost-shopify` | `/blog#email-marketing-cost-shopify` | How Much Should Email Marketing Cost for a Shopify Brand? |
| `how-ai-email-marketing-works` | `/blog#how-ai-email-marketing-works` | How AI Email Marketing Works for Shopify Brands |
| `klaviyo-contacts-not-converting` | `/blog#klaviyo-contacts-not-converting` | Why Your Klaviyo Contacts Aren't Converting |
| `managed-email-marketing-shopify` | `/blog#managed-email-marketing-shopify` | What Is Managed Email Marketing for Shopify? |
| `recover-lapsed-customers` | `/blog#recover-lapsed-customers` | How to Recover Lapsed Customers on Shopify with Email |
| `shopify-email-deliverability` | `/blog#shopify-email-deliverability` | How to Make Sure Your Shopify Emails Land in the Inbox (Not Spam) |
| `shopify-plateau` | `/blog#shopify-plateau` | Why Shopify Brands Stop Growing at 7 Figures (It's Not Your Ads) |
| `what-agency-should-deliver` | `/blog#what-agency-should-deliver` | What a Good Email Marketing Agency Should Actually Deliver |
| `win-back-campaign-shopify` | `/blog#win-back-campaign-shopify` | How to Set Up a Win-Back Email Campaign for Shopify Without an Agency |

## Category pages — PLANNED (not built)
Currently every category link (breadcrumbs, "View all →") points to the blog index as a no-404 stopgap. Real pages pending design (separate microsites, Option A):
- `/blog/revenue` — Revenue & Retention
- `/blog/agency` — Agencies & Hiring
- `/blog/klaviyo` — Klaviyo
- `/blog/verticals` — Verticals

## Cross-link graph (article → articles it links to)
- **agency-vs-hire-vs-ai-growth-marketer** → email-marketing-cost-shopify, what-agency-should-deliver, shopify-plateau
- **ai-flows-vs-manual-campaigns** → klaviyo-contacts-not-converting, shopify-email-deliverability, how-ai-email-marketing-works, recover-lapsed-customers
- **beauty-brands-email** → ai-flows-vs-manual-campaigns, shopify-email-deliverability, how-ai-email-marketing-works, recover-lapsed-customers
- **email-marketing-cost-shopify** → shopify-email-deliverability, agency-vs-hire-vs-ai-growth-marketer, managed-email-marketing-shopify, how-ai-email-marketing-works
- **how-ai-email-marketing-works** → klaviyo-contacts-not-converting, agency-vs-hire-vs-ai-growth-marketer, recover-lapsed-customers, managed-email-marketing-shopify
- **klaviyo-contacts-not-converting** → how-ai-email-marketing-works, shopify-email-deliverability, recover-lapsed-customers
- **managed-email-marketing-shopify** → klaviyo-contacts-not-converting, agency-vs-hire-vs-ai-growth-marketer, how-ai-email-marketing-works
- **recover-lapsed-customers** → how-ai-email-marketing-works, klaviyo-contacts-not-converting, managed-email-marketing-shopify
- **shopify-email-deliverability** → klaviyo-contacts-not-converting, recover-lapsed-customers, managed-email-marketing-shopify, how-ai-email-marketing-works
- **shopify-plateau** → recover-lapsed-customers, ai-flows-vs-manual-campaigns, how-ai-email-marketing-works
- **what-agency-should-deliver** → ai-flows-vs-manual-campaigns, email-marketing-cost-shopify, agency-vs-hire-vs-ai-growth-marketer, managed-email-marketing-shopify
- **win-back-campaign-shopify** → recover-lapsed-customers, shopify-email-deliverability, how-ai-email-marketing-works
