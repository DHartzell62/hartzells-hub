# Hartzell's Heat & Air — Marketing Reference

## Google Ads
**Account:** 8853457008 | Scripts: `C:/Users/davew/build_*.py`

### Active Campaigns (as of March 2026)
| Campaign | Daily Budget | Focus |
|----------|-------------|-------|
| Competitor \| Comfortworks | $10 | OKC/statewide geo + HVAC |
| Competitor \| True Climate | $8 | Logan/Canadian/OKC |
| Competitor \| Shockley's | $10 | Canadian/OKC |
| Competitor \| Air Flow Technologies | $10 | Canadian County (Yukon/Mustang/El Reno) |
| Competitor \| Woodward (Fire & Ice + Comfort Zone) | $10 | Woodward area |
| **Total competitor spend** | **$48/day** | |

### Key Ad Copy Rules
- Headlines: 30 char max | Descriptions: 90 char max
- NO phone numbers in ad text (policy violation)
- Phone goes in call asset only
- Pinned H1/H2 for brand differentiation
- Always lead with CKenergy rebate in Canadian County

### UTM Parameters (standard)
| Channel | UTM |
|---------|-----|
| Google Ads | utm_source=google&utm_medium=cpc |
| Facebook | utm_source=facebook&utm_medium=social |
| Instagram | utm_source=instagram&utm_medium=social |
| Email | utm_source=email&utm_medium=email |
| SMS | utm_source=sms&utm_medium=sms |
| Website | utm_source=website&utm_medium=organic |

---

## SEO — Site Status (March 2026)
- **171 pages + 34 posts** published
- All pages have BreadcrumbList schema
- All service/geo pages have FAQPage schema + aggregateRating (4.8/262)
- Rank Math descriptions set on all key pages
- Sitemap: hartzellsheatair.com/sitemap_index.xml (submitted to GSC)

### Top SEO Pages
- `/geothermal-heat-pumps/` — main geo hub
- `/oklahoma-geothermal-rebates-2026/` — rebate hub
- `/ckenergy-geothermal-rebate-oklahoma/` — CKenergy specific
- `/hvac-services-canadian-county-ok/` — Canadian County
- `/ac-repair-kingfisher-ok/` — core service

### SEO Priorities (ongoing)
- Keep rebate amounts current (utilities change rates)
- Monitor review count — update from 262 when it changes
- Blog: 34 posts, no new schema needed

---

## Analytics
| Tool | ID |
|------|----|
| GA4 | G-N72ZPDMCN8 |
| GTM | GTM-PQLKLWTG |
| Google Ads | AW-957557034 |
| Meta Pixel | 579261759276413 |
| Microsoft Clarity | vsnls4mdb6 |

**Key GA4 events:** `ads_conversion_Contact_Us_1`, `conversion_event_phone_call_lead`
**Looker Studio:** "Hartzell's Weekly Dashboard" — weekly email Mondays

---

## Lead Capture
- **Geo giveaway page:** hartzellsheatair.com/win-free-hvac-plan/
  - Prize: Dave's 360 Plan ($360 value)
  - Monthly drawing, central OK geo homeowners
  - Submissions → Zapier webhook → SMS to Dave
  - Fields captured: name, phone, email, address, zip, geo units, utility company

---

## SMS / Twilio
- **Account SID:** ACa0b1b2012d58d68592a41f28f7a59262
- **Sending #:** +14058050738
- **Messaging Service SID:** MGd252e45a5727034cd64185ebbe538f8d (A2P registered)
- Spring campaign script: `C:/Users/davew/build_sms_campaign.py`
- PMA sequence script: `C:/Users/davew/run_pma_sequence.py`

---

## Zapier
- **API key:** db811c3b16f54dbbb3f56c4e5f43eae4
- **Webhook:** https://hooks.zapier.com/hooks/catch/2745910/u0mi00f/
- Use cases: appointment reminders, review requests, estimate follow-ups, giveaway leads

---

## Key Differentiators (use in all marketing)
1. IGSHPA Accredited — engineered geo loops
2. ClimateMaster GeoElite Dealer — top dealer tier
3. CKenergy rebate knowledge — $2,000/ton (max $24,000) in Canadian County
4. 45 years HVAC experience
5. 4.8 stars / 262 reviews
6. Master HVAC License + NATE Certified
7. $111 diagnostic credited toward repair
8. Same-day service available

---

## Competitor Landscape (summary)
See `competitors.md` for full detail.

**Primary threats:**
- Comfortworks (OKC, geothermal, no IGSHPA)
- True Climate (Guthrie, Logan County)
- Air Flow Technologies (24 yrs Canadian County, lists Kingfisher)
- Wall Geothermal (OKC geo, engineering background, wrong rebate data)
- Hollifield Service Co. (Central OK, same IGSHPA + GeoElite certs)

**Advantage:** No competitor matches IGSHPA + ClimateMaster GeoElite + current accurate rebate knowledge + 262 reviews.
