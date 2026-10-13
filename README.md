# DMIT Hong Kong VPS: Tier 1 vs Eyeball vs Premium, Full Plan Prices, and Which One to Buy

If you searched for a Hong Kong VPS and landed on DMIT's store, the confusion is almost certainly the same one everyone hits: three "routing profiles," a stack of plan names in English, and prices running from $6.90 a month to $239.90 a month. The instinct is to compare CPU and RAM first. That's the wrong order here. In DMIT's Hong Kong lineup, the specs are broadly similar across tiers. The thing you're actually paying for is the route your packets take, and the price difference between the cheapest and most expensive option at the same hardware level is not small.

Here's the breakdown, with the plan data pulled from the store itself, so you can decide in one pass instead of three.

## What DMIT is selling in Hong Kong

DMIT is a US-registered provider (DMIT, Inc.) that has been running VPS services since around 2017, with data centers in Los Angeles, Hong Kong, and Tokyo. The Hong Kong node sits at Equinix HK2, and every plan is KVM virtualisation on AMD EPYC hardware with SSD storage, one IPv4 address, and an IPv6 /64 block included. Setup is free.

That's the part where the plans are the same. Where they diverge is the network profile, and DMIT splits Hong Kong into three of them:

- **Tier 1 (T1)** — international transit, no optimisation for mainland China. Cheap, big ports, huge traffic allowances.
- **Eyeball (EB)** — a middle profile aimed at mainland residential broadband, currently flagged as Beta by DMIT itself.
- **Premium (Pro)** — the flagship. Includes Tier 1 transit plus premium providers, explicitly including China Telecom's CN2 GIA.

Payment options are practical for a lot of buyers: cards, PayPal, Alipay, and WeChat Pay are all accepted.

## The three routes, in plain terms

If the acronyms mean nothing to you yet, the short version is that mainland China's three carriers each have a premium international path, and those paths cost the hosting provider real money.

**CN2 GIA** is China Telecom's top-tier global network (AS23764). It's the most expensive way to get traffic into and out of China, and it's the reason Pro plans cost what they do. **CMI** is China Mobile International, and **AS9929** is China Unicom's premium line. A "three-network optimised" Hong Kong VPS usually means it holds premium capacity on all three, so users don't degrade depending on which ISP they're on.

Tier 1 is a different animal entirely. It rides international carriers including RETN, with routing tuned toward Europe and general international interconnect. It is genuinely good at what it is built for, and it is not built for mainland China.

> If your visitors are in mainland China, buying Tier 1 to save money is the single most common mistake with this provider. The specs look identical to a Pro plan at a fifth of the price, and the experience is not.

## HKG Premium (AS3): full plan list and current prices

Premium is the profile that includes Tier 1 transit plus the premium providers, with China Telecom CN2 GIA named directly in the product description. These are the AS3-generation plans, running AMD EPYC 7003 series chips, all with 1 IPv4 + 1 IPv6 /64 and a 1Gbps port.

| Plan | vCPU | RAM | SSD | Traffic / month | Port | Price / month | Order |
| --- | --- | --- | --- | --- | --- | --- | --- |
| HKG.AS3.Pro.TINY | 1 | 1.0 GB | 20 GB | 500 GB | 1 Gbps | $39.90 | [ Start with the Pro entry plan](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=premium&aff=12046) |
| HKG.AS3.Pro.STARTER | 1 | 2.0 GB | 40 GB | 1000 GB | 1 Gbps | $79.90 | [ Compare the Pro STARTER specs](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=premium&aff=12046) |
| HKG.AS3.Pro.MINI | 2 | 4.0 GB | 60 GB | 1500 GB | 1 Gbps | $126.90 | [ See the Pro MINI configuration](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=premium&aff=12046) |
| HKG.AS3.Pro.MICRO | 4 | 4.0 GB | 80 GB | 2000 GB | 1 Gbps | $179.90 | [ Check the Pro MICRO pricing](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=premium&aff=12046) |
| HKG.AS3.Pro.MEDIUM | 4 | 8.0 GB | 160 GB | 2500 GB | 1 Gbps | $239.90 | [ View the Pro MEDIUM plan](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=premium&aff=12046) |

Two things worth noticing in that table. First, the jump from STARTER to MINI adds $47 for one extra core, 2GB of RAM, 20GB of disk, and 500GB of traffic. Second, traffic scales far more slowly than price: MEDIUM costs six times what TINY costs and gives you five times the traffic. If you're buying Pro, you're buying routing quality, not volume.

## HKG Tier 1 (AS3): the volume play

Tier 1 is where the numbers get strange. Ports start at 4Gbps and go to 10Gbps. Traffic allowances are measured in terabytes. And when you burn through your monthly allowance, the server does not stop — it drops to a throttled unmetered rate and keeps serving.

| Plan | vCPU | RAM | SSD | Traffic / month | Port | Overage rate | Price | Order |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| HKG.AS3.T1.WEE | 1 | 1.0 GB | 20 GB | 1000 GB | 4 Gbps | Unmetered @ 50 Mbps | $36.90 / year | [ Grab the annual WEE plan](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |
| HKG.AS3.T1.TINY | 1 | 1.0 GB | 20 GB | 2000 GB | 4 Gbps | Unmetered @ 100 Mbps | $6.90 / month | [ See the cheapest monthly T1 plan](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |
| HKG.AS3.T1.STARTER | 1 | 2.0 GB | 40 GB | 4000 GB | 10 Gbps | Unmetered @ 100 Mbps | $12.90 / month | [ Compare the T1 STARTER option](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |
| HKG.AS3.T1.MINI | 2 | 2.0 GB | 60 GB | 8000 GB | 10 Gbps | Unmetered @ 100 Mbps | $21.90 / month | [ Check the T1 MINI specs](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |
| HKG.AS3.T1.MICRO | 4 | 4.0 GB | 80 GB | 16 TB | 10 Gbps | Unmetered @ 200 Mbps | $32.90 / month | [ View the T1 MICRO plan](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |
| HKG.AS3.T1.MEDIUM | 4 | 8.0 GB | 160 GB | 32 TB | 10 Gbps | Unmetered @ 200 Mbps | $49.90 / month | [ Check the T1 MEDIUM pricing](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |
| HKG.AS3.T1.LARGE | 8 | 16 GB | 320 GB | 64 TB | 10 Gbps | Unmetered @ 500 Mbps | $99.90 / month | [ See the T1 LARGE configuration](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |
| HKG.AS3.T1.GIANT | 8 | 24 GB | 640 GB | 128 TB | 10 Gbps | Unmetered @ 1 Gbps | $199.90 / month | [ View the T1 GIANT plan](https://www.dmit.io/cart.php?region=hong-kong&generation=as3&network=tier-1&aff=12046) |

The first three rows — WEE, TINY, and STARTER — match what the store currently displays. The larger configurations reflect DMIT's recent Hong Kong listings, so confirm the spec sheet on the order page before you commit, since stock and configurations get reshuffled in waves.

WEE is annual-only at $36.90, which works out to just over $3 a month for 1TB of monthly traffic on a 4Gbps port. Nothing else in the Hong Kong market that carries a real local IP comes close on raw numbers. TINY at $6.90 monthly is the cheapest way to get a Hong Kong machine from this provider without paying a year up front.

## Eyeball: read the Beta label before you plan around it

Eyeball is the third profile, sitting between the two above. It leans on China Mobile's international path with direct handling where it helps, and DMIT has described it as a reasonable-effort optimisation for mainland access rather than a Premium equivalent.

The complication is status. DMIT has marked the Hong Kong Eyeball network as Beta, with a note that routes and performance may keep changing and that it isn't recommended for production environments with strict stability requirements. Inventory has also come and gone — at times it's been restocked alongside the other profiles, at other times it hasn't been available at all. Reported pricing when it has been in stock has run from $39.90/month for the AS3 entry plan up to $239.90 for the AS3 MEDIUM, with a higher-spec AN5 platform starting around $149.90/month.

If Eyeball is what you need, [👉 check whether HKG Eyeball stock is open right now](https://www.dmit.io/aff.php?aff=12046) rather than trusting any list, including this one.

## Where the money actually goes: price per gigabyte

This comparison tends to settle the argument faster than any spec sheet. Take the two mid-range plans:

- **HKG.AS3.T1.MINI** — $21.90 for 8000 GB. That's roughly **$0.0027 per GB**.
- **HKG.AS3.Pro.TINY** — $39.90 for 500 GB. That's roughly **$0.08 per GB**.

Tier 1 hands you about 30 times more traffic per dollar. That gap isn't a trick or a discount. It's the cost of CN2 GIA capacity, and it's the whole reason the two product lines exist at different price points. If you mainly need a Hong Kong IP, a fast port, and a lot of data, you are overpaying badly on Premium. If your users are on China Telecom and you care about round-trip latency, Tier 1's gigabytes are worthless to you.

## What happens when you exceed your traffic

This detail matters more than most reviews give it credit for, because it changes how you design your setup.

Tier 1 plans throttle instead of stopping. WEE falls to an unmetered 50Mbps, the smaller tiers to 100Mbps, and the big ones to 500Mbps or 1Gbps. Your server keeps responding, your backups keep running, and your site stays online at reduced speed until the cycle resets. For anything that can survive a slow month, that's a much safer failure mode than a hard cutoff.

Premium is reported to behave differently — several plan write-ups state that Premium traffic overage results in account suspension rather than throttling. DMIT's own product pages don't spell this out as clearly as the Tier 1 unmetered line, so if your workload is unpredictable, verify the overage policy on the order page before you buy.

## Which plan actually fits your job

Ignore the tier names for a second and answer one question: where are your users?

**Users outside mainland China.** Tier 1, and the decision becomes purely about size. TINY at $6.90/month handles a small site or a dev box. MINI at $21.90 with 8TB and a 10Gbps port is the sweet spot for APIs, mirrors, and anything that pushes real data. If you're moving large volumes, MICRO at $32.90 doubles both cores and traffic for $11 more — that's the cheapest upgrade in the whole HK lineup.

**Users in mainland China, budget is the constraint.** Eyeball if it's in stock and you accept the Beta caveat. If it isn't, understand that the honest fallback is Premium, not Tier 1. Buying T1 for a China-facing site is money spent on the wrong product, and no amount of hardware spec compensates for it.

**Users in mainland China, performance is the point.** Premium, and the entry plan is usually enough. HKG.AS3.Pro.TINY at $39.90/month gives 500GB of monthly traffic over CN2 GIA. For a business site or a SaaS dashboard with Chinese users, 500GB goes a long way, and $39.90 is a normal monthly bill for hosting that actually loads. Step up to STARTER at $79.90 only when you've measured that you need the extra gigabyte of RAM or the extra 500GB.

**Heavy compute or databases.** Pro MEDIUM at $239.90 for 4 vCPU / 8GB is a lot of money for a modest spec sheet, and the honest read is that you should look at the newer AN5 platform plans DMIT has introduced on the Premium line before defaulting to AS3. Different hardware generation, same routing profile.

**You just want a cheap Hong Kong IP.** HKG.AS3.T1.WEE at $36.90 for a full year is the answer, with the caveat that it's annual-only and throttles to 50Mbps once you pass 1TB in a month.

## Discount codes: what's actually live

Several coupon-tracking sites currently say the same thing, and it's worth repeating plainly: there is no publicly working DMIT coupon at the moment, and the low prices you see are already promotional pricing rather than list pricing waiting for a code.

That doesn't mean DMIT never discounts. The store has run recurring-discount campaigns, including an annual 45%-off code tied to a Hong Kong Tier 1 hardware upgrade promotion that was restricted to STARTER and above on the annual term. That campaign page is now marked as ended. If you're hoping for a code, the realistic move is to check the promotions page at checkout rather than trusting a coupon list that was scraped months ago.

On billing terms: T1 WEE is annual-only, and most other plans are available monthly. Longer commitments have historically been cheaper per month, but only where the store offers the term — verify at checkout instead of assuming.

## Test the route before you pay

Every Hong Kong plan is reachable for latency testing, and for a purchase this size it's worth ten minutes of your time:

- **Premium test IP:** 103.117.100.199
- **Tier 1 test IP:** 154.12.176.28
- **Eyeball test IP:** 154.12.188.3 (when in stock)

DMIT also runs a public Looking Glass at lg.dmit.sh where you can pull routes by hand. Third-party reviewers who have tested the Hong Kong Premium line report China-wide averages in the low 40ms range, with tier-one cities nearer 30–45ms and minimal packet loss. Treat that as a sample, not a promise — your own traceroute from your own ISP is the only number that describes your situation.

## Practical notes before checkout

The order page lets you customise RAM, SSD, and transfer on some configurations, so the base price isn't always the final price. Free setup applies, and each instance comes with one IPv4 and an IPv6 /64. DMIT's Hong Kong Premium plans are the ones that tend to sell out first when restocks happen, and restocks happen in waves rather than being continuously available.

If you're still deciding between the tiers, the fastest way in is to look at the two product groups side by side: [👉 open the Hong Kong plan list and compare them directly](https://www.dmit.io/aff.php?aff=12046).

## Verdict

The Hong Kong lineup at DMIT isn't complicated once you strip the marketing language off it. Tier 1 is an international-traffic machine with absurd traffic-to-dollar ratios and no mainland optimisation. Premium is the same hardware with CN2 GIA capacity bolted on, at roughly thirty times the cost per gigabyte. Eyeball is a reasonable middle, when you can get it.

Spend your money on the route that matches your users, then buy the smallest plan in that route that covers your traffic. What you should not do is buy Tier 1 because the numbers look better, if the people loading your site are in China. That's the one mistake this whole lineup is designed to punish.
