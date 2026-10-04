# ebay proxies: picking one IP per seller account, rotating IPs for listing research, and what the plans actually cost

Type "ebay proxies" into a search box and you're usually dealing with one of two problems. Either you run more than one store and you're tired of watching accounts get linked and restricted, or you need listing and sold-price data at a volume that gets you throttled or blocked from a single address. Those two problems want opposite things from the same tool, and a surprising amount of the advice out there blurs them together.

Here's the split, the ebay-specific rules that actually matter, and where 9Proxy's plans land in it — with the current price list, because the IP-based tiers changed on June 1, 2026.

## Why eBay links accounts in the first place

eBay doesn't need a single smoking gun. It accumulates signals:

- **IP address.** Two Seller Hub logins from the same office Wi-Fi on the same afternoon is one of the oldest detection patterns there is.
- **Browser fingerprint.** Same Chrome profile, same canvas and font set, different accounts.
- **Login geography.** A US-registered seller account that appears from a new country every few days.
- **Shared details.** Payment method, bank account, phone number, shipping address.
- **Identity verification.** Once you've passed KYC with the same name, address and tax ID, those accounts are tied together on eBay's side regardless of which proxy or device you used to log in.

That last one is the part most "stealth account" articles gloss over. A proxy changes your network identity. It doesn't change your legal identity, and it doesn't create permission.

> eBay allows multiple accounts only in specific situations — separate brands or business units are the usual examples. A clean residential IP helps accounts stay separate in practice. It does not make duplicate accounts compliant. Read eBay's own account-linking policy for the site you sell on, and treat any guide that promises a proxy is a "pass" as marketing.

## Two jobs, two completely different proxy settings

This is where most eBay setups go wrong. An account wants to stay put. A scraper wants to move.

| Job | Proxy type | Rotation | Billing model that fits |
| --- | --- | --- | --- |
| Daily Seller Hub logins across several stores | Fixed or long-sticky residential / ISP, one per account | None — same exit every day | Per IP, unlimited bandwidth |
| A VA or team logging into a store from abroad | Same country as the store | None | Per IP |
| Monitoring hundreds of listings and sold prices | Rotating residential | Fresh IP per request, short sticky while paging one listing | Per GB |
| Checking how a listing renders on ebay.de or ebay.co.uk | Residential in that country | Sticky, short | Either |
| A one-off region peek | Free list, read-only | — | Free |

The rule that saves money: use the cheapest tier the job tolerates, and step up only when blocks prove you need to.

And keep the two workflows apart. Running a listing scraper from the same IP you use to log into Seller Hub mixes your research traffic into your seller identity — which is exactly the kind of pattern that gets a store flagged.

**Match the proxy country to the eBay site.** US store → US IP, ebay.co.uk → UK, ebay.de → Germany, ebay.com.au → Australia, ebay.fr → France. Wrong country means wrong fee display, wrong shipping options, and occasionally a security challenge.

**Size accounts by the account, not the pool.** One dedicated IP per store, never shared between two stores, ideally on different subnets.

## Where 9Proxy fits

9Proxy is a residential proxy network — 20M+ residential IPs across 90+ countries, HTTP/HTTPS and SOCKS5, with targeting down to country, city, ZIP and ISP level on the by-IP side. It's not a datacenter or ISP-static product, and that distinction matters for eBay work, so let's be precise about it.

There are two residential models:

**Residential by IP.** You buy a number of IPs, each with unlimited bandwidth. You pick the location, forward a port, and traffic runs through that exit. Unused IPs never expire. The catch: residential IPs have natural uptime measured in hours up to roughly 24 hours, not forever. If you need an address that is literally the same for six months, this isn't an ISP proxy and it doesn't pretend to be — but for accounts, the practical approach is a sticky session plus the auto-rotation port feature, and the desktop app handles the forwarding for you.

**Residential by GB.** You buy traffic instead of addresses. The pool rotates — dynamic per request or sticky sessions — and you generate endpoints from the dashboard with username/password or IP whitelist. 180-day validity, unlimited on the enterprise tiers. This is the one that maps to listing and sold-price scraping.

Practical features worth knowing before you buy:

- **Auto-refresh** detects an offline IP and replaces it within about 60 seconds, which matters when a scraper is mid-run and a node drops.
- **The "Today List"** lets you reuse any IP that comes back online within 24 hours at no extra charge. 9Proxy puts the savings at roughly 20–30% on recurring work, which is plausible if your targets repeat.
- **60-second replacement.** If a proxy won't connect in the first minute, you can swap it out instead of eating the loss. Residential pools churn; this is the sane way to handle it.
- **Access paths.** A Windows desktop (Proxy Program) that routes at the OS level, Proxy2Web for zero-install browser use with user:pass, a ProxyHub line for mobile device management, and a public API for scripted control. Anti-detect browsers — Dolphin Anty, AdsPower, BitBrowser, Multilogin — work over SOCKS5.
- **Support** runs 24/7 over Telegram, email and tickets. On the by-IP model, though, there's no way around the desktop app for local port forwarding.

👉 [Start a 9Proxy account through the invite link](https://bit.ly/9-Proxy) if you want to test the pool against eBay before committing to a volume tier.

## Current pricing, in full

9Proxy raised IP-based and bundle prices on June 1, 2026 — the first adjustment since launch. GB-based packages were left untouched. Older reviews still quote the pre-June numbers ($0.20/IP entry, $25 Starter bundle), so ignore anything in that range as stale.

### IP-based packages (unlimited bandwidth per IP, unused IPs don't expire)

| Package | Per IP | Total | Purchase |
| --- | --- | --- | --- |
| 100 IPs | $0.24 | $24 | [Get 100 IPs](https://bit.ly/9-Proxy) |
| 500 IPs | $0.144 | $72 | [Get 500 IPs](https://bit.ly/9-Proxy) |
| 1,000 + 500 bonus IPs | $0.084 | $126 | [Get 1,500 IPs](https://bit.ly/9-Proxy) |
| 2,500 IPs | $0.084 | $210 | [Get 2,500 IPs](https://bit.ly/9-Proxy) |
| 5,000 IPs | $0.072 | $360 | [Get 5,000 IPs](https://bit.ly/9-Proxy) |
| 15,000 IPs | $0.048 | $720 | [Get 15,000 IPs](https://bit.ly/9-Proxy) |
| 25,000 IPs | $0.035 | $863 | [Get 25,000 IPs](https://bit.ly/9-Proxy) |
| 50,000 IPs | $0.029 | $1,438 | [Get 50,000 IPs](https://bit.ly/9-Proxy) |
| 100,000 IPs (Business) | $0.023 | $2,300 | [Get 100,000 IPs](https://bit.ly/9-Proxy) |
| 200,000 IPs (Business) | $0.021 | $4,140 | [Get 200,000 IPs](https://bit.ly/9-Proxy) |
| 500,000 IPs (Business) | $0.018 | $8,625 | [Get 500,000 IPs](https://bit.ly/9-Proxy) |

### GB-based packages (rotating pool, dashboard-generated endpoints)

| Package | Per GB | Total | Validity | Purchase |
| --- | --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | 180 days | [Buy 5 GB](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | $2.10 | $105 | 180 days | [Buy 55 GB](https://bit.ly/9-Proxy) |
| 100 GB | $1.50 | $150 | 180 days | [Buy 100 GB](https://bit.ly/9-Proxy) |
| 200 GB | $1.00 | $200 | 180 days | [Buy 200 GB](https://bit.ly/9-Proxy) |
| 1,000 GB | $0.80 | $800 | 180 days | [Buy 1,000 GB](https://bit.ly/9-Proxy) |
| 2,000 GB | $0.75 | $1,500 | 180 days | [Buy 2,000 GB](https://bit.ly/9-Proxy) |
| 3,000 GB (Enterprise) | $0.72 | $2,160 | No expiry | [Buy 3,000 GB](https://bit.ly/9-Proxy) |
| 6,000 GB (Enterprise) | $0.70 | $4,200 | No expiry | [Buy 6,000 GB](https://bit.ly/9-Proxy) |
| 10,000 GB (Enterprise) | $0.68 | $6,800 | No expiry | [Buy 10,000 GB](https://bit.ly/9-Proxy) |

### Bundle packages (IPs plus traffic, 180-day traffic validity)

| Bundle | Contents | Price | Purchase |
| --- | --- | --- | --- |
| Starter | 100 IPs + 5 GB | $30 | [Buy the Starter bundle](https://bit.ly/9-Proxy) |
| Popular | 1,500 IPs + 50 GB | $180 | [Buy the Popular bundle](https://bit.ly/9-Proxy) |
| Pro | 5,000 IPs + 500 GB | $720 (listed at $860, 16.28% off) | [Buy the Pro bundle](https://bit.ly/9-Proxy) |

One structural point in 9Proxy's favour for uneven e-commerce work: everything is balance-based, so a package you buy today doesn't evaporate at the end of a billing month. Traffic from bundles and GB packs sits valid for 180 days.

## Which package makes sense for an eBay operation

Ran through real scenarios rather than "it depends":

- **Three stores, one VA logging in daily.** The 100-IP package at $24 is the entry point, and it's overkill on paper. But you're buying address diversity, not just addresses: 100 IPs means you can give each store its own IP, keep a spare set for a fourth store, and rotate off any address that starts drawing verification prompts. $24 with unlimited bandwidth beats a metered plan the moment you start uploading listing photos through the proxy.
- **Agency running client stores across regions.** 500 IPs at $72 covers a few dozen accounts with real geographic matching — US, UK, DE, AU — plus room to retire dirty addresses without buying more.
- **Listing and sold-price research.** Don't buy IPs for this. A 100 GB pack at $150 handles a lot of eBay pages, since listing pages are light; the 200 GB tier at $200 drops you to $1/GB. You're paying for rotation, not for addresses you'll never reuse.
- **Both, in one budget.** The Popular bundle at $180 gives you 1,500 IPs for accounts plus 50 GB for research, and keeps the two traffic types from competing.

If your volumes are genuinely large — resellers, hundreds of stores, always-on monitoring — the Business IP tiers and the no-expiry enterprise GB tiers are the ones where the per-unit cost stops being the constraint.

## Setting it up without linking your own stores

1. **Buy the package that matches the job**, then open the dashboard. By-IP work runs through the desktop app with port forwarding; by-GB work can be used straight from the dashboard.
2. **Set the port range first.** In the app, define your starting port and how many ports you need before you start assigning, otherwise you'll be reassigning later.
3. **Filter by location properly** — country, then state or city, and postcode or IP range if you're hunting a specific market. Match it to the eBay site.
4. **Pin an account to one exit.** For any store you log into, use a sticky session on the same IP every day, complete 2FA on that IP, and don't casually open Seller Hub from your raw office connection in between.
5. **One browser profile per store.** AdsPower, Dolphin Anty or Multilogin — whichever you use, the profile and the IP travel together. A separate proxy with a shared Chrome profile still leaks fingerprint-level links.
6. **Keep research on separate credentials.** Rotating GB-based credits for scraping, sticky IPs for logins, never the same exit for both.
7. **Warm new accounts slowly.** Normal listing updates, human-paced messages, no mass automation in week one.
8. **Start listing checks at 20–40 pages per hour** and watch the block rate. eBay is less aggressive than Amazon, but bulk speed still trips it. When you do get throttled, the auto-refresh replacing dead nodes in ~60 seconds keeps the run from stalling.

## Where it's a weaker fit

Being straight about the limits, since eBay sellers get burned by mismatches rather than bad providers:

- **No true static ISP product.** If your requirement is one address that stays frozen for a year, look at a dedicated ISP proxy. 9Proxy's by-IP addresses rotate on residential timelines.
- **The by-IP model depends on a desktop app.** Running it purely server-side isn't the intended flow.
- **Pool size is mid-market.** 20M+ is fine for eBay work and clean on Tier 1 targets, but third-party comparisons put budget pools at 85–92% success on harder Tier 2 targets against 96%+ for larger providers. If you're scraping something heavily defended, budget accordingly.
- **City-level depth is called "limited"** in comparison write-ups against big-pool competitors, even though 9Proxy advertises city, ZIP and ISP targeting. Worth verifying against your exact target city before buying a large tier.

## What reviewers say

Mollified by the fact that there isn't a lot of independent testing on the record: Geekflare's 2026 review covers the post-adjustment pricing without disputing the model, and iTWire's write-up rates it around 9/10 while flagging the mandatory app, trial availability via support promotions rather than a self-serve button, and weaker results on streaming services like Netflix. On G2 there's a single review — 5 stars, from a cloud security architect who used it for regional security validation testing. One review is one review; don't treat it as consensus. On AlternativeTo, a user running Dolphin Anty and AdsPower reported stable IPs and reasonable pricing against other providers.

## Quick answers

**Do I need a proxy for one store from home?** No. One account, one country, home internet — you're fine. Add one when you add stores, remote staff, or automation.

**Can I use free proxies for eBay?** Not for anything you care about. Free lists are shared, dirty and short-lived; for a stealth account it's worse than nothing, because the IP may already be attached to banned accounts. Free lists are for a read-only region check while you test your scraper's plumbing.

**Does a proxy mean my second account is allowed?** No. It changes network identity, not eBay's rules or your KYC record.

**Sticky or rotating?** Accounts: sticky, permanently. Scraping: rotating, per request, with a short sticky window while paging a single listing.

**How do I know it works on eBay before buying a big tier?** Buy the smallest tier, run your actual workflow for a week, and measure block rate per region. 9Proxy's refund-on-failed-proxy policy and non-expiring IPs make that a cheap test rather than a commitment.

👉 [Set up an account and test the pool on your own eBay targets](https://bit.ly/9-Proxy) — the invite link attaches the referral code automatically at sign-up.

The honest summary: for eBay, the proxy is the easy part. One IP per seller account, country-matched, paired with an isolated browser profile, and rotating residential traffic kept on entirely separate credentials for research. Get that split right and a $24 hundred-IP package covers more stores than most people running "stealth" setups actually need. Get it wrong — two stores on one IP, or a scraper sharing your Seller Hub exit — and no provider on the market will save the accounts.
