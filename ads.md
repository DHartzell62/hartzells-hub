# Google Ads — Hartzell's Heat & Air

*Last updated: March 2026*

---

## Account
- **Account ID:** 885-345-7008
- **Login:** dave@hartzellsheatair.com
- **GA4:** G-N72ZPDMCN8
- **Google Ads conversion:** AW-957557034
- **Previous agency:** Equipped Marketing — UNLINKED March 2026

---

## Active Campaigns

### Core Service Campaigns
| Campaign | Budget/day | Notes |
|----------|------------|-------|
| HHA – Repair – Kingfisher | $25 | Main repair — weather-boosted |
| Search \| AC Repair \| Kingfisher OK | $30 | Location bid adjustments by area |
| Search \| HVAC Replacement \| Kingfisher OK | $20 | Install/replacement focus |
| Search \| Geothermal Repair \| Oklahoma Statewide | $15 | Full state, no city exclusions |
| HHA - Brand Protection \| 2026 | $10 | Brand keyword defense |
| Mini-Split \| Ductless \| Oklahoma \| 2026 | $15 | Ramping |
| HVAC Service \| Blaine & Major County \| 2026 | $15 | 6 ad groups |
| Spring Tune-Up \| Past Customers \| 2026 | $15 | Customer match remarketing |
| **Core total** | **~$145/day** | |

### Competitor Campaigns
| Campaign | Budget/day | Target |
|----------|------------|--------|
| Competitor \| Comfortworks | $10 | OKC / statewide geo |
| Competitor \| True Climate | $8 | Logan / Canadian / OKC |
| Competitor \| Shockley's | $10 | Canadian / OKC |
| Competitor \| Air Flow Technologies | $10 | Canadian County (Yukon/Mustang/El Reno) |
| Competitor \| Woodward (Fire & Ice + Comfort Zone) | $10 | Woodward area |
| **Competitor total** | **$48/day** | |

**Grand total: ~$193/day (~$5,800/month)**

---

## Auction Insights (last checked March 2026)
| Competitor | Impression Share | Overlap Rate | Above You |
|------------|-----------------|-------------|-----------|
| integrityheatandair.com | 13.06% | 22.17% | 43.11% |
| Hartzell's | 12.54% | — | — |
| comfortwave.com | <10% | 9.16% | 51.08% |
| suntechokc.com | <10% | 6.45% | 25.95% |
| asapheatandair.com | <10% | 9.11% | 44.86% |

---

## Local Services Ads (LSA)
- **Budget:** $435/week | **Target CPL:** $85
- **12-month results:** 333 charged leads | $68/lead avg | 27+ leads/month
- 176 maintenance leads (53%) — high PMA conversion opportunity
- OOS cities removed: Harrah, Choctaw, Luther, Spencer, Del City, Midwest City, Moore

---

## Location Bid Adjustments (local campaigns)
| Area | Adjustment |
|------|-----------|
| Kingfisher County | +30% |
| Hennessey / Okarche | +25% |
| Watonga / Fairview | +20% |
| ZIP 73099 (Yukon) | +20% |
| Enid / Guthrie / El Reno | +15% |
| Yukon / Mustang / Edmond | +10% |

**Negative locations:** Harrah, Choctaw, Luther, Spencer, Del City, Midwest City, Moore

---

## Ad Copy Rules
- Headlines: **30 chars max** | Descriptions: **90 chars max**
- **NO phone numbers in ad text** — policy violation; phone goes in Call Asset only
- Competitor names can appear in **keywords only** — never in ad copy
- Use "See Why We Rate Higher" type language for competitor ad groups
- Always lead with CKenergy rebate ($2,000/ton) in Canadian County copy

---

## Campaign Segmentation (Negative Keyword Firewalls)
- AC/repair campaigns → block geothermal terms
- Geo campaign → block AC repair terms
- All non-mini-split campaigns → block mini-split / ductless terms
- All campaigns → block competitor brand terms (except their dedicated campaign)
- All competitor campaigns → block "hartzell" terms (brand campaign owns those)

---

## Competitor Ad Copy Angles
| Competitor | Lead With |
|------------|-----------|
| Comfortworks | IGSHPA + ClimateMaster GeoElite — installs, repairs, AND maintenance |
| True Climate | IGSHPA + OEC rebates $700/ton in Logan County |
| Shockley's | CKenergy $2,000/ton up to $24,000 in Canadian County |
| Air Flow Technologies | 45 yrs experience, NATE certified, geothermal specialist |
| Fire & Ice / Comfort Zone | 24/7 availability (they're M-F 8-5 only), IGSHPA accredited |

---

## Conversion Tracking
| Conversion | Type | Status |
|------------|------|--------|
| Calls from ads | Google Ads | Primary |
| Click Phone calls | GA4 import | Primary |
| Contact Us | GA4 import | Primary |
| Booking click | GA4 import | Primary |

---

## Weather-Triggered Budget Script
- File: `C:/Users/davew/weather_rules.js` — runs daily 6:00 AM via Google Ads Scripts
- Uses Open-Meteo API (free) — Kingfisher coords 35.8556, -97.9328
- ≤60°F → heating campaigns +75% | 70-79 → AC +25% | 80-89 → AC +50% | ≥90 → AC +100%

---

## Weekly Reporting
- **GA4 report:** `ga4_weekly_report.js` → Google Apps Script → emails Monday 7 AM
- **Ads report:** `weekly_report_script.js` → Google Ads Scripts → Monday 7 AM
- **Looker Studio:** "Hartzell's Weekly Dashboard" → auto-emails Monday (dave@hartzellsheatair.com)

---

## Competitor Conquesting Ad Group
- Lives inside: HHA – Repair – Kingfisher campaign
- Keywords: integrity heat and air, comfortwave okc, suntech okc, asap heat and air
- RSA pinned: "Top-Rated Kingfisher HVAC" pos 1 | "4.8 Stars / 262 Reviews" pos 2
- Landing page: /ac-repair-kingfisher-ok
- Rule: cannot use competitor names in ad copy — use "See Why We Rate Higher" etc.

---

## Brand Protection
- Campaign: HHA - Brand Protection | 2026
- 14 exact + phrase keywords on all "hartzell" name variations
- **Trademark:** Path clear to file "HARTZELL'S HEAT & AIR" in IC 037 (~$250 at uspto.gov/trademarks/apply)

---

## Pending / To-Do
- [ ] Search terms audit — run every 7 days; flag negatives, find new keywords
- [ ] Switch HVAC Replacement + Geo Statewide to Maximize Conversions after 30 days data
- [ ] Add Mini-Split exclusions to all other campaigns
- [ ] Spring Tune-Up: verify USER_LIST audience size (needs 1,000+ for search remarketing)
- [ ] Trademark filing — IC 037 at uspto.gov (~$250)
- [ ] Meta remarketing campaign — Pixel live, build homeowner audience
- [ ] ElevenAgents AI voice — inbound call triage after-hours (start after SMS A2P approved)
- [ ] GBP API access — submit at support.google.com/business/contact/api_default

---

## Hiring Campaign
- Campaign: HHA – Hiring – HVAC / Geothermal
- Always-on recruiting — not weather-boosted
- Targets HVAC techs and geo installers

---

## Direct Outreach Campaigns

### Campaign 1: Geo Owner Free PMA (March 2026)
**Target:** 46 existing geo customers with mobile in HCP
**Offer:** Free Geo Basic PMA ($360 value) — 1 year, no charge
**Goal:** 20+ bookings, loop inspections → find rebuild/replacement opportunities
**Send date:** March 20 | **Close:** April 15
**List:** 48 unique geo customers in HCP | 46 mobile | 36 email

**SMS #1 (send March 20, 9–10am):**
```
Hi [Name]! Dave from Hartzell's. We're giving existing geo owners a FREE year of Geo Basic PMA ($360 value). Loop inspection + maintenance included. Interested? Reply YES or: [link]
```

**SMS #2 (YES response — same day):**
```
Awesome! You're locked in for a FREE Geo Basic PMA year. Pick a time here: [booking link] — or call 405-375-4822.
```

**SMS #3 (MAYBE/tell me more — within 24 hrs):**
```
Geo Basic PMA includes: annual loop inspection, pressure check, filter replacement, system diagnostics, priority service. $360 value, free to you. Book here: [link] or call 405-375-4822.
```

**SMS #4 (no response — day 3):**
```
No pressure! FREE Geo Basic PMA offer ends April 15. When you're ready: [link]
```

**Email follow-up (non-SMS responders — March 27):**
Subject: Your free geo inspection is waiting — $360 value
Body: personalized offer, bullet list of what's included, book link, expires April 15.

**Success targets:**
| Metric | Target |
|--------|--------|
| SMS sent | 46 |
| Response rate | 65% (30 people) |
| Bookings | 20+ |
| Inspections completed | 16+ |
| Geo installs from inspections | 5 |

**Revenue impact:** 20 × $360/yr = $7,200 recurring + 5 installs × ~$25K = ~$125K

---

### Campaign 2: Geo Giveaway — New Prospects
**Target:** Rural homeowners — Canadian, Blaine, Kingfisher, Logan, Oklahoma Co
**Offer:** Win a free Geo 360 PMA ($499 value) — maintenance + loop repressurization
**Channel:** Facebook ads
**Landing page:** /win-free-hvac-plan/ (update prize to Geo 360)
**Timeline:** Launch March 25 | Run through June 30 | Draw winner July 1
**Goal:** 50+ entries, 50+ email subscribers, 1+ geo install from pipeline

**Non-winner follow-up sequence:**
1. Draw day: "You didn't win — here's 25% off your first geo assessment"
2. +1 week: "Here's how much you could save with a geo system"
3. +2 weeks: "Can we give you a free energy audit?"

---

## Key Scripts
| Script | Purpose |
|--------|---------|
| `ads_orchestrator.py` | Claude-powered Google Ads orchestrator |
| `build_airflow_campaign.py` | Air Flow Technologies competitor campaign |
| `build_woodward_campaign.py` | Fire & Ice + Comfort Zone Woodward campaign |
| `build_blaine_major_rsa.py` | Blaine & Major County ad groups |
| `generate_minisplit_campaign.py` | Mini-split bulk upload (5 CSVs) |
| `weather_rules.js` | Weather-triggered budget script |
| `ga4_weekly_report.js` | GA4 weekly email (Apps Script) |
| `weekly_report_script.js` | Ads weekly email (Ads Scripts) |
