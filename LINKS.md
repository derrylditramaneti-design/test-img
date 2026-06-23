# YoboLabs link registry

> Single source of truth for cross-page links. **Update this file whenever you add, move, or rename a page** so links in the main site and sub-pages stay correct.
> Referenced from code via: `<!-- Links registry: .../LINKS.md -->`

_12 articles, each a dedicated microsite on the Global site (converted 2026-06-23)._

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
Each article is now its **own microsite on the Global site**, served at `https://global.pages.yobolabs.ai/<slug>` with server-rendered per-article SEO/OG (real social previews). The blog index links straight to these; legacy `/blog#<slug>` deep links auto-redirect to the real URL. To edit an article, edit its own microsite (the `/blog` index no longer embeds them).

| Slug | URL | Title |
|---|---|---|
| `agency-vs-hire-vs-ai-growth-marketer` | https://global.pages.yobolabs.ai/agency-vs-hire-vs-ai-growth-marketer | Email Marketing Agency vs. Full-Time Hire vs. AI Growth Marketer |
| `ai-flows-vs-manual-campaigns` | https://global.pages.yobolabs.ai/ai-flows-vs-manual-campaigns | AI Flows vs. Manual Campaigns: Which Drives More Revenue? |
| `beauty-brands-email` | https://global.pages.yobolabs.ai/beauty-brands-email | AI Email Marketing for Shopify Beauty Brands: What's Working in 2026 |
| `email-marketing-cost-shopify` | https://global.pages.yobolabs.ai/email-marketing-cost-shopify | How Much Should Email Marketing Cost for a Shopify Brand? |
| `how-ai-email-marketing-works` | https://global.pages.yobolabs.ai/how-ai-email-marketing-works | How AI Email Marketing Works for Shopify Brands |
| `klaviyo-contacts-not-converting` | https://global.pages.yobolabs.ai/klaviyo-contacts-not-converting | Why Your Klaviyo Contacts Aren't Converting |
| `managed-email-marketing-shopify` | https://global.pages.yobolabs.ai/managed-email-marketing-shopify | What Is Managed Email Marketing for Shopify? |
| `recover-lapsed-customers` | https://global.pages.yobolabs.ai/recover-lapsed-customers | How to Recover Lapsed Customers on Shopify with Email |
| `shopify-email-deliverability` | https://global.pages.yobolabs.ai/shopify-email-deliverability | How to Make Sure Your Shopify Emails Land in the Inbox (Not Spam) |
| `shopify-plateau` | https://global.pages.yobolabs.ai/shopify-plateau | Why Shopify Brands Stop Growing at 7 Figures (It's Not Your Ads) |
| `what-agency-should-deliver` | https://global.pages.yobolabs.ai/what-agency-should-deliver | What a Good Email Marketing Agency Should Actually Deliver |
| `win-back-campaign-shopify` | https://global.pages.yobolabs.ai/win-back-campaign-shopify | How to Set Up a Win-Back Email Campaign for Shopify Without an Agency |

## Category pages (LIVE)
4 category microsites on the Global site. The blog index "View all →" links and each article's breadcrumb category link point here. Own SEO + OG image each.

| Category | URL | Articles |
|---|---|---|
| Revenue & Retention | https://global.pages.yobolabs.ai/category-revenue | shopify-plateau, recover-lapsed-customers, ai-flows-vs-manual-campaigns |
| Agencies & Hiring | https://global.pages.yobolabs.ai/category-agency | agency-vs-hire-vs-ai-growth-marketer, email-marketing-cost-shopify, what-agency-should-deliver |
| Email & Klaviyo Fundamentals | https://global.pages.yobolabs.ai/category-klaviyo | how-ai-email-marketing-works, klaviyo-contacts-not-converting, managed-email-marketing-shopify |
| Vertical Playbooks | https://global.pages.yobolabs.ai/category-verticals | beauty-brands-email, shopify-email-deliverability, win-back-campaign-shopify |

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
