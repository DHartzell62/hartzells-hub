# HCP (Housecall Pro) — Hartzell's Heat & Air

*Last updated: March 2026*

---

## Account
- **Plan:** MAX
- **Login:** dave@hartzellsheatair.com
- **API Key:** (stored in memory — not in public repo)
- **Reviews widget:** embed via iframe on any WP page

---

## Key Numbers
- **Total customers in HCP:** 2,593
- **2025 jobs:** 1,203 total | 799 completed | 305 user-canceled
- **2026 YTD (through Mar 15):** 165 jobs | 84 completed | $246,610 revenue

---

## Pricing in HCP
- All amounts stored in **cents** — $189.00 = `unit_price: 18900`
- Dispatch: $99 | Diagnostic: $111 | Tune-up: $229
- Emergency: $99 dispatch + $111 diagnostic + repair (all three collected)

---

## Job Statuses
| Status | Meaning |
|--------|---------|
| `scheduled` | Booked, not yet done |
| `in progress` | Tech on site |
| `complete unrated` | Done, no review yet |
| `complete rated` | Done, review received |
| `pro canceled` | Canceled by office |
| `user canceled` | Canceled by customer |

**Note:** `work_status='completed'` does NOT work in API — use `complete unrated` and `complete rated`.

---

## Booking & Dispatch Rules
- Confirm online bookings within 1 hour during business hours
- Call customer to confirm if same-day
- Default arrival window: 3 hours
- Tech confirms via HCP text 30 min before arrival
- Apply UTM source tag to every HCP job for lead tracking

---

## UTM / Lead Source Tags
| Source | HCP Tag |
|--------|---------|
| Google Ads | utm_source=google |
| Google organic | utm_source=website |
| Facebook/Instagram | utm_source=facebook / instagram |
| SMS campaign | utm_source=sms |
| Referral | tag: Referral |
| Geo giveaway | source: geo_giveaway |

---

## Maintenance Plans (PMA)

| Plan | Price/yr | HCP Page ID |
|------|----------|-------------|
| Tune-Up PMA | $138 | 2804 |
| Basic PMA | $189/yr or $15.75/mo | 2805 |
| Dave's 360 | $360/yr or $30/mo | 2806 |
| Geo Basic | $360 | — |
| Geo Plus | $428 | — |
| Geo 360 | $499 | — |
| WH Tune-Up | — | 2868 |

**PMA rule:** Dispatch waived ONLY on the included annual maintenance visit. Repair calls = $99 every time.

**After sale:** Enter as recurring job in HCP → send plan PDF → schedule first visit.

---

## Discounts in Pricebook

| Discount | Amount | Trigger |
|----------|--------|---------|
| Annual Maintenance Loyalty | 5% | Consecutive annual maintenance customers |
| Welcome Back | $50 | Returning customer after 12+ months |
| Neighbor Referral | $50 | Referred by existing customer |
| Veteran / First Responder | 5% | Active/retired military, police, fire, EMT |
| Senior Courtesy | 5% | Customer age 65+ |
| Maintenance Club Member | 10% (max $300) | Active PMA member |
| Decision Day | 5% | Approves repair same day as diagnosis |
| Multi-Repair | 5% | Multiple repairs on same visit |
| Cash / Check Courtesy | 3% on repairs over $2,000 | Ask before writing invoice |

**Expired — deleted from pricebook:** ENERGY STAR tax credit items (25C, 25D all expired Dec 31, 2025)

---

## JB Warranties (JBW) — Pricebook Items

| Item | Retail |
|------|--------|
| AC System — 10yr P&L Plus | $1,299 |
| AC System — 5yr P&L Plus | $649 |
| Heat Pump — 10yr P&L Plus | $1,299 |
| Furnace — 10yr P&L Plus | $749 |
| Furnace — 5yr P&L Plus | $549 |
| Mini-Split 1-Zone — 10yr P&L Plus | $549 |
| Mini-Split 1-Zone — 5yr P&L Plus | $449 |
| Mini-Split Additional Zone (add-on) | $199 |
| Geothermal HP — 10yr P&L Plus | $1,399 |
| Geothermal HP — 5yr P&L Plus | $995 |
| Water Heater — 10yr P&L Plus | $349 |
| Water Heater — 8yr P&L Plus | $299 |
| Water Heater — 6yr P&L Plus | $249 |
| Tankless WH — 10yr P&L Plus | $649 |

---

## Pricebook Format (flat rate — all sections)
1. Service name
2. Retail price
3. Cost
4. Average install time
5. Technician notes
6. Optional bundled packages at end of section

**File structure:** Category | Name | Description | Price | Task Code | Pro Tip — alphabetical by Category then Name.

**Trane Bundles:** Pending definition (system + JBW warranty combos, good/better/best tiers)

---

## Automations (via Zapier + HCP)
- Booking confirmation → sent automatically on book
- Appointment reminder → 30 min before via HCP text
- Review request → auto-sent when job marked complete
- 3-day follow-up → if no review
- Estimate follow-up → day 7 if open estimate not responded to

---

## API Limits
- No pricebook read/write API — CSV import only (HCP Admin → Pricebook → Materials → Import)
- Available endpoints: GET /jobs, /jobs/{id}/line_items, /customers, /employees, /estimates, /company
- Script files: `C:/Users/davew/build_hcp_discounts.py`, `build_jbw_pricebook.py`
- CSV exports: `C:/Users/davew/Downloads/`

---

## 14-Day Diagnostic Credit Tracking
- Customer has 14 days to accept estimate and apply $111 credit to invoice
- HCP flags open estimates — follow up at day 7 if no response
- Credit applies to repair OR replacement (it is a credit, NOT a refund)
