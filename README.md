# Hourly VPS too pricey? Cheap hourly VPS options on Vultr explained — plan tiers, lowest hourly rate, and how to pick the right size (full pricing table included)

Last Tuesday at 2am I needed a Linux box for exactly four hours. Not a year, not a month — four hours, to run a one-off script against a 3GB dataset. Renting a "real" monthly VPS for that job would have been like buying a house to spend a weekend in. That little situation is the whole reason cheap hourly VPS exists, and it's the reason I keep a Vultr tab open in my browser pretty much permanently.

## What cheap hourly VPS actually means

Cheap hourly VPS is a virtual private server you rent and pay for by the hour instead of by the month — spin it up, use it, destroy it, and you only owe for the hours it actually ran. No annual commitment, no cancellation dance. The cheapest hourly VPS plans hover around half a cent per hour, which means a 10-hour testing session can cost you less than a cup of coffee.

On Vultr specifically, the lowest published hourly rate right now is $0.004/hr on the IPv6-only Regular Performance Cloud Compute plan. Multiply that out and a full 28-day cycle (672 hours) caps at $2.50/month — so the "hourly" billing never costs more than the monthly sticker price. That cap is the key detail most comparison articles skip, and it's the reason hourly billing is genuinely safe to leave running.

## Why Vultr shows up on every "cheap hourly VPS" shortlist

There are maybe a dozen providers that bill by the hour. Most of them either cap the savings badly, charge a setup fee, or quietly round up to full days. Vultr does none of those things, and the spec sheet reads like someone actually listened to developers.

- **Real per-hour pricing with a monthly cap.** You pay $0.004–$0.005/hr on the entry tier and the meter stops at the monthly rate. No surprises.
- **32+ data centers worldwide**, including spots in Tokyo, Seoul, Mumbai, São Paulo, Johannesburg — so latency isn't a reason to pick a pricier provider.
- **Hourly billing across every product line**, not just the cheap one. Cloud Compute, High Frequency, Optimized Cloud Compute, even Cloud GPU all bill by the hour.
- **New-user promo credit.** Vultr runs a $200 free credit offer for new accounts (use code `FLYTWOHUNDRED` on the coupons page), which effectively makes your first ~50,000 hours of the $0.004 plan free. Treat it as a trial, not a permanent discount.

Vultr's own marketing claims the newer VX1 plans deliver "up to 82% better performance per dollar compared to leading hyperscaler cost efficiency-optimized compute plans." Take vendor benchmarks with salt, but the pricing pressure on AWS and DigitalOcean is real — I've personally migrated cron jobs off DO to Vultr and cut the bill by roughly 40% for identical specs.

👉 [Check Vultr's current plans and promo credits](https://www.vultr.com/?ref=9738262-9J)

## The full Vultr hourly plan lineup (so you don't have to dig)

Here's where most "cheap VPS" articles cheat — they list three or four plans and call it a day. Vultr has three Cloud Compute families plus a dedicated Optimized Cloud Compute tier, and the hourly rates swing wildly between them. Picking the wrong family can triple your bill.

### Cloud Compute — Regular Performance (the cheap seats)

Powered by previous-gen Intel CPUs and regular SSD. This is where the cheapest hourly VPS rates on the entire platform live. Use it for low-traffic sites, blogs, dev/test boxes, small databases.

| Plan | vCPU | RAM | Bandwidth | Storage | Monthly | Hourly | Get it |
|---|---|---|---|---|---|---|---|
| IPv6 Only | 1 | 0.5 GB | 0.50 TB | 10 GB | $2.50 | $0.004 |  [Start at $2.50/mo](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| Entry | 1 | 0.5 GB | 0.50 TB | 10 GB | $3.50 | $0.005 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 1GB | 1 | 1 GB | 1.00 TB | 25 GB | $5 | $0.007 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2GB | 1 | 2 GB | 2.00 TB | 55 GB | $10 | $0.015 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2 vCPU / 2GB | 2 | 2 GB | 3.00 TB | 65 GB | $15 | $0.022 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 4GB | 2 | 4 GB | 3.00 TB | 80 GB | $20 | $0.030 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 8GB | 4 | 8 GB | 4.00 TB | 160 GB | $40 | $0.060 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 16GB | 6 | 16 GB | 5.00 TB | 320 GB | $80 | $0.119 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 32GB | 8 | 32 GB | 6.00 TB | 640 GB | $160 | $0.238 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 64GB | 16 | 64 GB | 10.00 TB | 1280 GB | $320 | $0.476 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 96GB | 24 | 96 GB | 15.00 TB | 1600 GB | $640 | $0.952 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |

If your goal is literally the cheapest hourly VPS you can find anywhere, the $0.004/hr IPv6-only plan is the floor. It's so cheap that forgetting it on for a full month still costs you less than a fast-food meal.

### Cloud Compute — High Performance (AMD EPYC / Intel Xeon + NVMe)

Same idea, modern hardware. AMD and Intel pricing happens to match here, so I'm listing once. NVMe SSD and current-gen CPUs make a real difference for I/O-heavy workloads.

| Plan | vCPU | RAM | Bandwidth | Storage | Monthly | Hourly | Get it |
|---|---|---|---|---|---|---|---|
| 1GB | 1 | 1 GB | 2.00 TB | 25 GB | $6 | $0.009 |  [Get High Performance](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2GB | 1 | 2 GB | 3.00 TB | 50 GB | $12 | $0.018 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2 vCPU / 2GB | 2 | 2 GB | 4.00 TB | 60 GB | $18 | $0.027 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 4GB | 2 | 4 GB | 5.00 TB | 100 GB | $24 | $0.036 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 8GB | 4 | 8 GB | 6.00 TB | 180 GB | $48 | $0.071 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 12GB | 4 | 12 GB | 7.00 TB | 260 GB | $72 | $0.107 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 16GB | 8 | 16 GB | 8.00 TB | 350 GB | $96 | $0.143 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 24GB | 12 | 24 GB | 12.00 TB | 500 GB | $144 | $0.214 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |

For about $0.009/hr you jump from regular SSD to NVMe — that's worth it for almost any database workload.

### Cloud Compute — High Frequency (3GHz+ Intel Xeon + NVMe)

For latency-sensitive stuff: game servers, real-time APIs, trading bots. Same price as the AMD/Intel High Performance tier, but tuned for clock speed over core count.

| Plan | vCPU | RAM | Bandwidth | Storage | Monthly | Hourly | Get it |
|---|---|---|---|---|---|---|---|
| 1GB | 1 | 1 GB | 1.00 TB | 32 GB | $6 | $0.009 |  [Get High Frequency](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2GB | 1 | 2 GB | 2.00 TB | 64 GB | $12 | $0.018 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2 vCPU / 2GB | 2 | 2 GB | 3.00 TB | 80 GB | $18 | $0.027 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 4GB | 2 | 4 GB | 3.00 TB | 128 GB | $24 | $0.036 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 8GB | 3 | 8 GB | 4.00 TB | 256 GB | $48 | $0.071 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 16GB | 4 | 16 GB | 5.00 TB | 384 GB | $96 | $0.143 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 24GB | 6 | 24 GB | 6.00 TB | 448 GB | $144 | $0.214 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 32GB | 8 | 32 GB | 7.00 TB | 512 GB | $192 | $0.286 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 48GB | 12 | 48 GB | 8.00 TB | 768 GB | $256 | $0.381 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |

### Optimized Cloud Compute — dedicated vCPU plans

These run on fully dedicated AMD EPYC vCPUs (no noisy neighbors) and split into four flavors: General Purpose, CPU Optimized, Memory Optimized, Storage Optimized. Hourly rates start at $0.042/hr and scale up to roughly $5.71/hr on the largest General Purpose box.

| Family | Cheapest hourly | Cheapest monthly | Best for | Get it |
|---|---|---|---|---|
| General Purpose | $0.045/hr | $30/mo | Web/app servers, e-commerce, game servers |  [Browse General Purpose](https://www.vultr.com/products/optimized-cloud-compute/?ref=9738262-9J) |
| CPU Optimized | $0.042/hr | $28/mo | Video encoding, CI/CD, HPC, analytics |  [Browse CPU Optimized](https://www.vultr.com/products/optimized-cloud-compute/?ref=9738262-9J) |
| Memory Optimized | $0.060/hr | $40/mo | MySQL, Memcached, in-memory caches |  [Browse Memory Optimized](https://www.vultr.com/products/optimized-cloud-compute/?ref=9738262-9J) |
| Storage Optimized | $0.112/hr | $75/mo | Cassandra, MongoDB, OLTP workloads |  [Browse Storage Optimized](https://www.vultr.com/products/optimized-cloud-compute/?ref=9738262-9J) |

The Optimized tier is where "cheap" stops being the right word — these are production-grade dedicated vCPU machines. But the same hourly logic applies: spin one up for a 3-hour load test, tear it down, owe $0.13. That's the magic.

👉 [Compare all Vultr plans side by side](https://www.vultr.com/?ref=9738262-9J)

## The cheapest hourly VPS plan, examined up close

The $0.004/hr IPv6-only Regular Performance plan deserves its own section because it's the headline number that pulls people in. Here's what you actually get for it.

**Specs:** 1 vCPU, 0.5 GB RAM, 0.50 TB bandwidth, 10 GB regular SSD storage. IPv6 only — no IPv4 address included, which is the catch. If whatever you're running needs to be reachable from a legacy IPv4 network (and a lot of corporate networks still are), you'll need to add a reserved IPv4 address for an extra ~$3/month.

**Realistic cost math:**
- Pure hourly, no IPv4: $0.004 × 730 = $2.92/month uncapped → billed $2.50/month
- With IPv4 added: roughly $5.50/month equivalent, billed hourly on the IPv4 portion too
- For a 4-hour one-off job: about $0.02

That last line is the entire pitch. Two cents to run a script for an afternoon.

**Where it actually works:** cron jobs that ping an endpoint, a tiny monitoring bot, a personal WireGuard endpoint, a CI runner for a low-traffic repo, a sandbox to test a config change before pushing it to a real box.

**Where it breaks:** anything that needs more than 0.5 GB RAM (so, basically anything running a modern Node app or a database bigger than a toy), and anything that needs IPv4 inbound without paying extra.

If you're new and want to test the waters without spending a dime, the new-user $200 promo credit covers this plan for about 50,000 hours of usage — more than enough to decide if Vultr fits your workflow.

👉 [Claim Vultr's $200 free credit and test the $0.004/hr plan](https://www.vultr.com/?ref=9738262-9J)

## How to spin up your first cheap hourly VPS (5 steps)

This is the actual workflow I use when I need a throwaway box. Should take you under five minutes the first time.

1. **Sign up and add the promo code.** Create the account, then on the billing screen enter `FLYTWOHUNDRED` to claim the $200 credit. Verify your card — Vultr does a small auth hold, doesn't charge it.
2. **Pick Products → Cloud Compute.** From the control panel, click the "+" deploy button and choose Cloud Compute. Regular Performance is the cheap hourly VPS family; High Performance adds NVMe for ~$0.005/hr more.
3. **Choose your spec and region.** Pick the smallest plan that fits your workload — the 1 vCPU / 1GB at $0.007/hr is the sweet spot for most quick jobs. Choose a region close to you or your users; the price is identical across all 32+ locations.
4. **Select OS and any startup script.** Ubuntu 22.04 LTS is the safe default. If you want the box to auto-configure on boot, paste a cloud-init script in the Startup Script field — install Docker, pull your repo, start the service.
5. **Deploy and watch the meter.** Click Deploy. The instance is live in ~30 seconds. The hourly meter starts the moment it's active. When you're done, hit Destroy in the control panel — billing stops immediately. Snapshots cost $0.05/GB/month if you want to save the box for later.

That's the whole game. The discipline is just remembering to destroy instances you don't need. I keep a Slack reminder that pings me every Friday: "nuke any Vultr boxes you forgot about."

## Picking the right plan by scenario (not by spec sheet)

Reading spec sheets is the slow way to choose. Faster: match your scenario to a tier.

**"I just need to run a script for an afternoon."**
→ Regular Performance, 1 vCPU / 1GB at $0.007/hr. Total cost: a few cents. Don't overthink it.

**"I'm hosting a low-traffic personal blog or portfolio."**
→ Regular Performance, 1 vCPU / 2GB at $0.015/hr (~$10/month). Enough headroom for WordPress or a static site generator with a backend.

**"I need a database that won't fall over."**
→ High Performance, 2 vCPU / 4GB at $0.036/hr (~$24/month). NVMe SSD is the upgrade that actually matters here — disk I/O is what kills cheap VPS databases.

**"I'm running a game server for friends."**
→ High Frequency, 4 vCPU / 16GB at $0.143/hr (~$96/month). Minecraft, CS2, Valheim all want clock speed and RAM, and the 5TB bandwidth covers a small private server comfortably.

**"I'm doing CI/CD builds and need consistency."**
→ Optimized Cloud Compute — CPU Optimized, 2 vCPU / 4GB at $0.060/hr (~$40/month). Dedicated vCPU means no neighbor noise during your build window.

**"I need to load-test a production app for 2 hours."**
→ Optimized Cloud Compute — General Purpose, 8 vCPU / 32GB at $0.357/hr. Two-hour test = ~$0.71. Try doing that on AWS without a calculator and a panic attack.

## What real users actually say

I'll be straight with you — Vultr isn't universally beloved, and any review that pretends otherwise is selling you something. Here's the unfiltered picture from places I trust.

On **r/VPS**, the recurring sentiment is that Vultr sits in the sweet spot between Hetzner's rock-bottom pricing and DigitalOcean's polish. A typical thread comment: "I've used Vultr and Hetzner, both are great" — Hetzner wins on raw price for sustained monthly use, Vultr wins on global region coverage and hourly billing across all tiers. That matches my own experience: Hetzner's hourly billing is real but their data center footprint is mostly Europe.

On **r/selfhosted**, there's a long-running thread complaining about Vultr's 2024 terms-of-service update that briefly claimed broad commercial rights over customer content. Vultr walked it back after backlash, but it left a mark on community trust. If you're hosting anything sensitive, snapshot to external storage and read the current TOS yourself before assuming anything.

On **Trustpilot**, Vultr sits at a mixed rating — positive reviews praise provisioning speed and the breadth of regions, negative reviews cluster around payment disputes and account-suspension issues that seem to hit users from certain regions harder. Treat the promo credit as a genuine trial: deploy, test, and if you decide to stay, fund the account with a method that won't trip their fraud filters.

The honest summary: Vultr is excellent for cheap hourly VPS use cases — short-lived dev boxes, testing, low-traffic production — and you should think twice before putting mission-critical workloads on any single cloud without backups elsewhere. That's not a Vultr-specific caveat, it's just cloud hygiene.

👉 [Try Vultr with $200 free credit and decide for yourself](https://www.vultr.com/?ref=9738262-9J)

## Handling the price objection (because someone's going to ask)

"If Vultr is so cheap, why does my bill keep creeping up?"

Three reasons, in order of how often I see them:

1. **Orphaned instances.** You spun up a box, got distracted, forgot it existed. The hourly meter didn't forget. Set up the destroy reminder, or use Vultr's API to auto-destroy instances older than X days.
2. **Snapshots you don't need.** $0.05/GB/month sounds tiny until you have 12 snapshots of a 40GB box sitting there for six months. That's $24 of pure waste.
3. **Bandwidth overages.** Each plan includes a bandwidth allowance; overages bill per GB. A game server with a viral clip can rack up overage fees faster than the VPS itself. Monitor bandwidth in the control panel.

The fix for all three is the same: treat Vultr's billing dashboard like a credit card statement. Check it weekly. Cheap hourly VPS only stays cheap if you're paying attention.

## Quick FAQ: the questions people actually search

**Is Vultr really billed hourly, or is it monthly with hourly math?**
Both. The meter runs per hour, but it caps at the monthly rate. So a $5/month plan costs at most $5 even if you ran it 730 hours. The hourly rate is just the monthly rate divided by 672 (28 days) for billing-cap purposes. Source: Vultr's own FAQ page confirms the 730-hour monthly billing model for compute products.

**What's the absolute cheapest hourly VPS on Vultr?**
The IPv6-only Regular Performance Cloud Compute at $0.004/hr ($2.50/month cap). Add a reserved IPv4 address for ~$3/month extra if you need IPv4 inbound.

**Does Vultr charge for stopped instances?**
No — but only if you destroy the instance. A "stopped" instance still holds its resources (CPU, RAM, storage, IP) and still bills. To stop billing, you must destroy the instance. Snapshots preserve the disk image for later restore.

**How does Vultr's hourly billing compare to DigitalOcean?**
Both bill hourly with a monthly cap. Vultr's entry price is lower ($2.50 vs DO's $4 minimum droplet), and Vultr bills hourly across more product lines including Cloud GPU. DigitalOcean's control panel and documentation are generally considered more polished. For cheap hourly VPS specifically, Vultr wins on floor price; DO wins on UX.

**Can I get a Vultr free trial without a credit card?**
You need a payment method on file for verification, but the $200 promo credit (code `FLYTWOHUNDRED`) means you don't have to spend your own money during the trial period. The credit covers select products and expires — check the coupons page for current terms.

## The bottom line

Cheap hourly VPS isn't a gimmick — it's a genuinely different way of paying for compute that makes sense any time your need is short, unpredictable, or experimental. Vultr's lineup covers the full price spectrum from $0.004/hr up to multi-dollar-per-hour GPU instances, all on the same hourly meter, all capped at monthly rates so you never get a surprise bill from leaving something on.

If you've never tried it, the lowest-risk move is to grab the new-user credit, deploy the $0.004/hr plan, run a single script, destroy the box, and look at the invoice. Two cents of billing has a way of clarifying whether this model fits your workflow better than any spec sheet can.

👉 [Get started with Vultr — $200 free credit for new users](https://www.vultr.com/?ref=9738262-9J)
