# 📋 EV Market 2026 — Full Insights Report
> Extracted from Power BI Dashboard | 4 Pages | 12 Visuals | 2,000 Records

---

## Page 1 — Sales & Market Share

### Visual 1: Brand vs Total Sales (Column Chart)
**Fields:** Brand (X-axis) × Sum of Annual_sales_units (Y-axis)

**Insights:**
- Tesla leads with **101,459,482 total units** — the highest of any brand by a wide margin.
- BYD is second at **50,472,617 units**, roughly half of Tesla's volume.
- Volkswagen is a close third at **48,186,657 units**, showing strong European presence.
- Kia (16.6M) and Hyundai (15.2M) form a strong Korean cluster in positions 4 and 5.
- There is a sharp drop-off after the top 3 brands — the market is highly concentrated.
- BMW, Ford, Mercedes, Audi, and GM/Chevrolet form a secondary mid-tier tier (2–8M units).

**Business Implication:** The EV market is an oligopoly at the top. Any new entrant must compete against Tesla's brand equity and BYD's cost advantage simultaneously.

---

### Visual 2: Market Segment Share (Donut Chart)
**Fields:** Market_segment (legend) × Sum of Annual_sales_units (values)

| Segment | Units Sold | Share |
|---|---|---|
| Premium | 86,507,799 | 33.4% |
| Mid-range | 83,479,890 | 32.2% |
| Luxury | 65,966,088 | 25.4% |
| Budget | 23,353,407 | 9.0% |

**Insights:**
- Premium and Mid-range together account for **65.6%** of all units sold.
- Luxury is surprisingly large at 25.4% — EVs are aspirational products.
- Budget is drastically underrepresented at 9% despite 151 listed models — volume per model is low.
- The market is skewed upmarket, suggesting EV adoption is still predominantly in middle-to-high income brackets.

**Business Implication:** A brand that successfully cracks the budget segment at scale (like BYD is attempting) could reshape the entire market distribution.

---

### Visual 3: Sales Growth Over Years (Line Chart)
**Fields:** Year (X-axis) × Sum of Annual_sales_units (Y-axis)

| Year | Total Sales |
|---|---|
| 2020 | 4,373,954 |
| 2021 | 11,762,346 |
| 2022 | 21,426,170 |
| 2023 | 40,791,903 |
| 2024 | 64,685,343 |
| 2025 | 87,603,840 |
| 2026 | 28,663,628 (partial year) |

**Insights:**
- Sales grew **~20× in 5 years** from 2020 to 2025.
- Year-over-year growth has been consistent: roughly doubling every 1.5–2 years.
- 2023 was a breakout year — sales nearly doubled vs 2022 (+90%).
- 2026 data is partial (dataset captured mid-year), so full-year projection could exceed 100M units.

**Business Implication:** The EV market is still in hyper-growth. Companies entering now are not too late — the market at full maturity is likely 3–5× larger than today.

---

## Page 2 — Pricing & Value Analysis

### Visual 1: Price vs Range (Scatter Chart)
**Fields:** Price_usd (X-axis) × Range_miles (Y-axis), colored by Brand

**Insights:**
- No strong linear correlation — paying more does not guarantee more range.
- **Lucid** and **Porsche** occupy the high-price zone but vary in range efficiency.
- Several mid-price brands (Honda, Mercedes) deliver competitive range at lower price points.
- **Tesla** models cluster in a "sweet spot" — high range at a relatively reasonable price.
- Outliers exist in both directions: overpriced short-range and underpriced long-range models.

**Business Implication:** Range-per-dollar is not a straightforward metric — brands that market "value efficiency" have a genuine opportunity to differentiate.

---

### Visual 2: Avg Price by Brand & Segment (Clustered Bar)
**Fields:** Brand (Y-axis) × Sum(Price_usd), series = Market_segment

**Top avg prices by brand:**
| Brand | Avg Price (USD) |
|---|---|
| Lucid | $192,517 |
| Porsche | $157,051 |
| Mercedes | $128,718 |
| BMW | $98,062 |
| Audi | $93,875 |
| Tesla | $93,523 |
| Rivian | $89,974 |
| Polestar | $89,828 |

**Insights:**
- Lucid and Porsche are outliers even within the luxury segment.
- Tesla's premium positioning at ~$93K is justified by volume — suggesting brand trust carries pricing power.
- Brands like Rivian and Polestar price near Tesla but with far lower sales — they need to earn the premium.
- BYD, despite high volume, sits in the lower-mid price range — a deliberate volume-first strategy.

---

### Visual 3: Price by Market Segment (Treemap)
**Fields:** Market_segment × Sum(Price_usd)

**Insights:**
- Premium segment has the largest block — highest total price mass in the market.
- Luxury follows closely, reflecting high per-unit prices despite fewer units.
- Mid-range and Budget occupy notably smaller tiles despite mid-range having strong unit sales.
- The treemap reveals: **revenue concentration in premium/luxury despite unit share being 65% mid/budget**.

**Business Implication:** EV manufacturers generate more revenue per unit in premium/luxury. Unit leadership (Tesla) does not fully translate to revenue dominance if pricing is not maximised.

---

## Page 3 — Customer & Geographic Insights

### Visual 1: Top 10 Models by Customer Rating (Clustered Column)
**Fields:** Model + Brand × Sum(Customer_rating), filtered to Top 10

| Rank | Brand | Model | Avg Rating |
|---|---|---|---|
| 1 | Mercedes | EQC | 3.86 |
| 2 | Volvo | XC40 Recharge | 3.86 |
| 3 | Mercedes | EQS | 3.83 |
| 4 | Porsche | Taycan | 3.83 |
| 5 | Mercedes | GLE EV | 3.82 |
| 6 | Porsche | Macan Electric | 3.81 |
| 7 | Tesla | Model 3 | 3.80 |
| 8 | Tesla | Model Y | 3.79 |
| 9 | Mercedes | EQG | 3.79 |
| 10 | Tesla | Model S | 3.79 |

**Insights:**
- Mercedes dominates customer satisfaction with 4 models in the Top 10.
- Volvo's XC40 Recharge ties for first — impressive for a Swedish brand with limited EV history.
- Tesla Model 3 and Model Y make the top 10 despite being mass-market — a quality signal.
- Ratings are clustered tightly (3.79–3.86), suggesting high baseline expectations across the industry.

---

### Visual 2: Body Type by Country (Stacked Column)
**Fields:** Country_of_origin × Count(Body_type), series = Body_type

| Country | Trucks | SUVs | Sedans | Coupes | Hatchbacks | Vans |
|---|---|---|---|---|---|---|
| US | 224 | 123 | 105 | 108 | 108 | 106 |
| Germany | 99 | 73 | 93 | 96 | 96 | 74 |
| South Korea | 43 | 100 | 42 | 42 | 45 | 46 |
| China | 55 | 44 | 56 | 46 | 64 | 48 |
| Sweden | 4 | 3 | 0 | 3 | 5 | 6 |
| Japan | 2 | 21 | 5 | 8 | 6 | 1 |

**Insights:**
- The **US specialises heavily in Trucks** (224 models — more than any other body type from any country).
- **South Korea leads in SUVs** (100 models), reflecting Kia/Hyundai's SUV-first EV strategy.
- **Germany** produces a balanced mix, especially Coupes (96) and Sedans (93) — consistent with European design tradition.
- **China** has the most Hatchbacks (64), targeting urban commuter utility.

---

### Visual 3: Brand × Segment Avg Price (Matrix Table)
**Fields:** Rows = Brand, Columns = Market_segment, Values = Avg(Price_usd)

**Insights:**
- The matrix reveals that many brands only compete in 1–2 segments, not across all four.
- Lucid and Porsche appear exclusively in Luxury — no affordable entry points.
- Tesla spans Premium and Mid-range — a multi-tier strategy enabling maximum addressable market.
- BYD operates in Budget and Mid-range — China's domestic market plays out in the data.

---

## Page 4 — Technology Insights

### Visual 1: Autopilot Level by Brand (Clustered Bar)
**Fields:** Brand × Count(Autopilot_level)

| Brand | Level 0 | Level 1 | Level 2 | Level 3 |
|---|---|---|---|---|
| Tesla | 0 | 0 | 315 | 119 |
| BYD | 150 | 98 | 34 | 0 |
| Volkswagen | 95 | 75 | 24 | 0 |
| Kia | 88 | 51 | 27 | 0 |
| BMW | 0 | 83 | 67 | 0 |
| Mercedes | 0 | 60 | 36 | 0 |
| Hyundai | 66 | 65 | 21 | 0 |
| Ford | 57 | 54 | 18 | 0 |

**Insights:**
- **Tesla is the only brand with Level 3 autonomy** (119 models) — a significant competitive moat.
- All of Tesla's fleet is at Level 2 or above — fully committed to autonomy as a product pillar.
- **BYD's 150 Level 0 models** confirm its focus on affordability, not autonomous features.
- BMW and Mercedes show more autonomy investment than volume brands (Kia, VW), reflecting premium tech positioning.

---

### Visual 2: Drive Type Distribution (Pie Chart)
**Fields:** Drive_type × Count(Drive_type)

| Drive Type | Count | Share |
|---|---|---|
| AWD | 754 | 37.7% |
| RWD | 678 | 33.9% |
| FWD | 568 | 28.4% |

**Insights:**
- AWD leads the market — consumers prioritise all-conditions handling and performance.
- RWD follows closely — preferred in performance and sports-oriented EVs.
- FWD is the least common — typically associated with budget/urban models.
- The AWD dominance aligns with the market's premium skew — most AWD EVs are mid-range or above.

---

### Visual 3: Range vs Charging Speed by Brand (Line & Column Combo)
**Fields:** Brand × Avg(Range_miles) [columns] + Sum(Charging_speed_kw) [line]

| Brand | Avg Range (mi) | Avg Charging Speed (kW) |
|---|---|---|
| Honda | 326.0 | 166.5 |
| Porsche | 274.9 | 279.3 |
| Mercedes | 270.8 | 125.9 |
| Toyota | 269.7 | 119.9 |
| Rivian | 268.7 | 116.1 |
| Volvo | 267.8 | 139.1 |
| Polestar | 267.6 | 128.3 |

**Insights:**
- **Honda leads in range** (326 mi avg) but has only moderate charging speed — optimised for distance, not speed.
- **Porsche leads in charging speed** (279.3 kW) but at shorter range — optimised for performance driving.
- Most brands cluster in the 260–270 mi / 115–130 kW zone — the current market standard.
- The combo chart reveals that **range and charging speed are not correlated** — brands make deliberate engineering trade-offs.

---

## ✅ Overall Conclusions

1. **The EV market is growing explosively** — 20× in 5 years — with no sign of slowdown.
2. **Tesla's dual advantage** (brand + autonomy tech) makes it uniquely hard to displace.
3. **Budget EVs are underserved** — a massive untapped opportunity for brands that can crack cost efficiency.
4. **Customer satisfaction is converging** — top-rated models span from mass-market (Tesla) to premium (Mercedes/Porsche).
5. **Autonomy is still nascent** — Level 3 is Tesla-exclusive; most of the world is still at Level 1.
6. **Geography shapes product** — US = trucks, Korea = SUVs, Germany = sedans, China = hatchbacks.
7. **AWD is the new default** — nearly 38% of all EVs, driven by consumer demand for all-season performance.

---

*Report generated from EV_SALES.pbix — 4 pages, 12 visuals — May 2026*
