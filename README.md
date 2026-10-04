# market research proxies: how to pull city-level pricing and competitor data without paying for bandwidth you don't use

Anyone typing this into a search bar usually already knows they need proxies. The awkward part comes next: per-gigabyte or per-IP billing? How many cities? Will a mid-priced pool survive a Cloudflare-protected retailer, or will you spend the afternoon solving CAPTCHAs instead of shipping the report?

Those questions have concrete answers, and they mostly depend on what your data collection actually looks like. Price sweeps, ad verification, SERP checks and panel-style geo testing look like the same job from the outside but bill very differently. Below is what to figure out first, where 9Proxy fits, and where it doesn't.

## What people mean by "market research proxies"

The phrase gets used for at least four different workflows, and they have almost nothing in common technically.

**Retail and e-commerce price intelligence.** You're pulling product pages, prices, stock labels and assortment from the same handful of domains, often for the same cities, repeatedly. Page weight is chunky and the targets usually sit behind bot protection. This is a bandwidth-heavy job that also needs the IP to look residential.

**Ad verification and localized content checks.** You want to see which creative a brand is running in Lyon versus Chicago, or whether a landing page redirects differently on a phone. Request volume is small; location accuracy is everything.

**SERP and SEO research.** Scraping search results or checking rankings as a local user. Thousands of tiny requests, frequent IP rotation, low data per request.

**Survey and panel routing checks.** Verifying that a questionnaire accepts the geo you claim, that pricing pages display the right currency, or that a form doesn't reject traffic from a given region. Small volume, high need for sticky sessions.

Written out like that, the pattern is obvious: two of these are bandwidth problems, and two are IP-identity problems. That single distinction decides which billing model makes sense.

## The billing model matters more than the price per unit

9Proxy splits residential access into two purchasing models, and the difference is structural, not cosmetic. Their documentation lays it out plainly:

|  | Residential by IPs | Residential by GB |
| --- | --- | --- |
| Billing | Fixed package, priced by IP count | Fixed package, priced by total traffic |
| Traffic | Unlimited during the IP's active window | Deducted by GB consumed |
| Endpoint generation | 1 IP = 1 usage when forwarded | Unlimited endpoints, only GB deducted |
| IP lifetime | A few hours up to 24h, varies per IP | Rotates per request or per session |
| Validity | Unused IP balance doesn't expire until activated | 180 days, unlimited on Enterprise tiers |
| Rotation | No natural rotation; Auto Rotation Proxy rotates on selected ports at custom intervals | Rotating or sticky mode built in |
| Auth | Desktop app with local port forwarding, optional proxy authentication | Username/password or IP whitelist |
| Setup | Desktop app required | Runs straight from the dashboard |

Read that table again with market research tasks in mind. The IP-based model behaves like a bucket of disposable local identities with no data ceiling. The GB model behaves like a traffic wallet with an unlimited supply of rotating endpoints.

Which one wins depends on one number: bytes per accepted record.

If a single product page load costs you half a megabyte and you're sweeping tens of thousands of them, per-GB billing turns your project budget into a moving target. If, instead, you're firing off lightweight API calls or SERP queries where each accepted response is a few kilobytes, per-IP packages are the wasteful choice, because you'd be buying identities you don't need and leaving their unlimited bandwidth on the table.

## Geographic targeting is the actual product

A residential proxy for market research isn't about hiding. It's about being seen as an ordinary shopper in a specific place.

9Proxy advertises 20+ million residential IPs across 90+ countries, with targeting down to country, state, city, ZIP code and ISP level. City and ZIP targeting is the part that matters here, because regional retail data doesn't align neatly with country borders. Same retailer, same day, three ZIP codes, three price points.

Two caveats worth checking against your own target list before you commit money:

- **90+ countries is not the widest coverage on the market.** Several competitors advertise 195+ locations. If your market research only touches the US, UK, Germany, Japan and Brazil, that gap is irrelevant. If you're doing genuine emerging-market work, verify your specific countries exist before buying.
- **Country-level coverage doesn't guarantee city-level inventory depth.** Test the exact metros you need rather than trusting a coverage list.

When you're ready to test that, you can 👉 [👉 open the 9Proxy sign-up and check the current package list](https://bit.ly/9-Proxy) — registration runs through an invite code, so use that link rather than the plain homepage.

## Every 9Proxy package, side by side

9Proxy adjusted IP-based and bundle pricing on June 1, 2026. Bandwidth pricing was left untouched, and there's no subscription requirement in any of these tiers.

| Plan | Model | What you get | Price (USD) | Validity / notes | Get it |
| --- | --- | --- | --- | --- | --- |
| 100 IPs | IP-based | 100 residential IPs, unlimited bandwidth | $24 | IPs never expire until activated | [ Get the 100 IP pack](https://bit.ly/9-Proxy) |
| 500 IPs | IP-based | 500 residential IPs, unlimited bandwidth | $72 | Same terms | [ Get the 500 IP pack](https://bit.ly/9-Proxy) |
| 1,000 + 500 IPs | IP-based | 1,500 residential IPs, unlimited bandwidth | $126 | Bonus IPs included | [ Get the 1,000 IP pack](https://bit.ly/9-Proxy) |
| 2,500 IPs | IP-based | 2,500 IPs, unlimited bandwidth | $210 | Same terms | [ Get the 2,500 IP pack](https://bit.ly/9-Proxy) |
| 5,000 IPs | IP-based | 5,000 IPs, unlimited bandwidth | $360 | Same terms | [ Get the 5,000 IP pack](https://bit.ly/9-Proxy) |
| 15,000 IPs | IP-based | 15,000 IPs, unlimited bandwidth | $720 | Same terms | [ Get the 15,000 IP pack](https://bit.ly/9-Proxy) |
| 25,000 IPs | IP-based | 25,000 IPs, unlimited bandwidth | $863 | Same terms | [ Get the 25,000 IP pack](https://bit.ly/9-Proxy) |
| 50,000 IPs | IP-based | 50,000 IPs, unlimited bandwidth | $1,438 | Same terms | [ Get the 50,000 IP pack](https://bit.ly/9-Proxy) |
| 100,000 IPs | Business IP | 100,000 IPs, unlimited bandwidth | $2,300 | High-volume tier | [ Get the 100,000 IP pack](https://bit.ly/9-Proxy) |
| 200,000 IPs | Business IP | 200,000 IPs, unlimited bandwidth | $4,140 | High-volume tier | [ Get the 200,000 IP pack](https://bit.ly/9-Proxy) |
| 500,000 IPs | Business IP | 500,000 IPs, unlimited bandwidth | $8,625 | High-volume tier | [ Get the 500,000 IP pack](https://bit.ly/9-Proxy) |
| 5 GB | GB-based | 5 GB of rotating residential traffic | $15 ($3.00/GB) | 180 days | [ Get the 5 GB pack](https://bit.ly/9-Proxy) |
| 55 GB | GB-based | 50 GB + 5 GB bonus | $105 ($2.10/GB) | 180 days | [ Get the 55 GB pack](https://bit.ly/9-Proxy) |
| 100 GB | GB-based | 100 GB | $150 ($1.50/GB) | 180 days | [ Get the 100 GB pack](https://bit.ly/9-Proxy) |
| 200 GB | GB-based | 200 GB | $200 ($1.00/GB) | 180 days | [ Get the 200 GB pack](https://bit.ly/9-Proxy) |
| 1,000 GB | GB-based | 1,000 GB | $800 ($0.80/GB) | 180 days | [ Get the 1,000 GB pack](https://bit.ly/9-Proxy) |
| 2,000 GB | GB-based | 2,000 GB | $1,500 ($0.75/GB) | 180 days | [ Get the 2,000 GB pack](https://bit.ly/9-Proxy) |
| 3,000 GB | Enterprise GB | 3,000 GB | $2,160 ($0.72/GB) | Traffic never expires | [ Get the 3,000 GB pack](https://bit.ly/9-Proxy) |
| 6,000 GB | Enterprise GB | 6,000 GB | $4,200 ($0.70/GB) | Traffic never expires | [ Get the 6,000 GB pack](https://bit.ly/9-Proxy) |
| 10,000 GB | Enterprise GB | 10,000 GB | $6,800 ($0.68/GB) | Traffic never expires | [ Get the 10,000 GB pack](https://bit.ly/9-Proxy) |
| Bundle: 100 IPs + 5 GB | Bundle | Mixed identity + traffic | $30 | Bundled traffic valid 180 days | [ Get the starter bundle](https://bit.ly/9-Proxy) |
| Bundle: 1,500 IPs + 50 GB | Bundle | Mixed identity + traffic | $180 | Bundled traffic valid 180 days | [ Get the mid bundle](https://bit.ly/9-Proxy) |
| Bundle: 5,000 IPs + 500 GB | Bundle | Mixed identity + traffic | $720 | Bundled traffic valid 180 days | [ Get the pro bundle](https://bit.ly/9-Proxy) |

Enterprise GB tiers also include team mode with one owner and up to five members, per-member traffic controls, shared non-expiring bandwidth, activity logs and unlimited share-code creation — worth knowing if your research team bills time to different clients.

## Doing the arithmetic before you pick a model

Nobody can hand you the right tier without knowing your page weights, so run the estimate yourself. The formula is boring:

**Monthly GB = requests per month × average accepted response size × retry factor**

The retry factor is the multiplier people forget. If a target blocks 10 percent of your attempts and you log every response including challenge pages, your effective data cost is higher than the accepted-record count suggests.

Here's the shape of it at two different scales, using the published prices above:

- **Light, high-rotation work** (SERP checks, small API polling, a few hundred price points): a 55 GB pack at $105 covers roughly two months of steady daily sweeps if you're burning about a gigabyte a day, and the 180-day validity means an idle fortnight doesn't waste anything.
- **Heavy catalog sweeping** (full product pages, images avoided, but chunky HTML across 20+ markets): once you're clearing several hundred gigabytes a month, per-GB columns stop being cheap. At that point the 500 IP pack at $72 with unlimited bandwidth looks strange on paper until you realise you're paying for identity, not for data.

The crossover isn't a fixed number — it moves with how many concurrent sessions you need and how clean those sessions have to stay. But the direction is consistent: **volume of bytes pushes you to IP-based, volume of rotations pushes you to GB-based.**

If your project genuinely needs both — sticky identities for basket-level follow-through and rotating power for catalog breadth — that's what the bundles exist for, and $180 for 1,500 IPs plus 50 GB undercuts buying those two things separately.

## Rotating versus sticky, in practice

Market research runs into a wall that generic scraping advice never mentions: session continuity changes the data.

Pull three prices from the same retailer with three different IPs in ten seconds and you may get three different results — not because the retailer has regional pricing, but because you kept restarting the session. Currency, shipping estimates, and personalized promotions can all snap to whatever the edge decides your session identity is.

The working pattern:

1. **Rotating** for breadth — category pages, search results, anything you're sampling once and discarding.
2. **Sticky** for continuity — any sequence of pages that must belong to one "shopper": basket flow, zip-code-scoped pricing, inventory by store.
3. **Log the exit identity** alongside each record. Without it you can't tell a genuine regional price difference from a session artifact, and your report ends up making a claim the data doesn't support.

9Proxy supports rotating and sticky modes on GB-based packages, and IP-based packages hold an IP for a few hours up to a day, with an Auto Rotation Proxy for scheduled switching on chosen ports.

## What independent testing actually shows

Published benchmarks for this provider land in different places depending on who ran them, which is normal — targets differ, so results differ.

Geekflare ran 300 sequential requests through rotating residential IPs against a major e-commerce platform sitting behind Cloudflare's bot protection: 293 successful passes (97.7 percent), 5 CAPTCHA challenges (all from one IP), 2 hard blocks, and a 0.63-second average response time. Directory-level benchmarks elsewhere record a 97 percent success rate with roughly 1.3-second average responses, and a hands-on case study reported around 99.5 percent success with ~0.6 seconds.

The honest read: on moderately protected retail targets, expect the vast majority of requests to land, expect occasional challenges, and treat latency as target-dependent. Budget for a retry layer regardless of provider. Anyone promising 100 percent success on protected retail sites is selling something other than proxies.

## Setup, and the one friction point

GB-based proxies need no software. You authenticate with username and password or an IP whitelist, and manage everything from the dashboard — which is why automation, headless scraping and server-side pipelines generally run on GB-based packages.

IP-based proxies historically required the 9Proxy desktop app for local port forwarding. The addition of Proxy2Web removed that constraint for browser retrieval, letting you grab IP-based proxies from a web interface instead of installing anything. There's also ProxyHub for mobile environments, with a Lite version for individual devices and a Pro version for managing multiple devices from one dashboard.

Protocol support covers HTTP, HTTPS and SOCKS5 on both models, so browsers, automation tools and custom scripts are all viable.

## Where 9Proxy is the wrong choice

Worth saying out loud, because it saves a refund request:

- **You need datacenter proxies for cheap, high-speed bulk on unprotected targets.** 9Proxy's product line is residential, and datacenter proxies are listed as coming soon, not available.
- **You need genuinely exhaustive country coverage.** 90+ countries, not 195+.
- **You want to buy without a desktop app on IP-based packages and don't want to use the web retrieval option.** Check your workflow first.
- **You need enterprise compliance documentation, ASN-level targeting or a dedicated account manager from day one.** Those features sit with larger, pricier providers.

For mid-sized research teams watching cost per accepted record, the trade-off usually works out. For heavily protected Tier 3 targets that demand 96 percent-plus success rates at scale, budget providers generally aren't the answer, and 9Proxy is a budget provider.

## A short checklist before you pay

1. Pick five representative URLs across your actual target mix — one easy, two moderate, one ugly, one that needs a sticky session.
2. Decide bytes per accepted record before choosing a model, not after.
3. Confirm your specific cities and ZIPs resolve before committing to a large IP pack.
4. Buy the smallest tier that covers your test. The 5 GB pack at $15 or the 100 IP pack at $24 is enough to learn whether the pool behaves on your targets.
5. Track acceptance rate, not HTTP status. A 200 response can still be a consent wall or an empty app shell.
6. Keep raw page weights and timestamps so a real price movement can be distinguished from a duplicate collection.

Testing at that scale costs less than a team lunch, and it tells you more than any comparison table — including this one.

## FAQ

**Do I need residential proxies for market research at all?**
Not always. Public databases and unprotected sites work fine on cheaper datacenter IPs. You need residential routing when the target applies bot protection, or when the data you want only appears to genuine local residential visitors.

**Is per-GB or per-IP cheaper for price monitoring?**
Per-GB for light, high-rotation tasks with small responses. Per-IP for anything pulling full pages at volume, because unlimited bandwidth during the IP's lifetime removes the ceiling. Model both against your own page weights before deciding.

**How long do 9Proxy's GB packages last?**
180 days on standard and most higher GB tiers, with unlimited validity on the 3,000 GB, 6,000 GB and 10,000 GB Enterprise packages. Unused IP-based balance doesn't expire until you activate it.

**Can I use these with my existing scraping stack?**
Yes — HTTP, HTTPS and SOCKS5 are supported, with username/password and IP whitelist authentication on GB-based packages. There's no lock-in to a proprietary collector.

The short version: the keyword gets you looking at proxy providers, but your own page weights and session requirements pick the plan. Work those two numbers out first, and the decision usually makes itself — 👉 [👉 compare the full 9Proxy package range before you commit](https://bit.ly/9-Proxy).
