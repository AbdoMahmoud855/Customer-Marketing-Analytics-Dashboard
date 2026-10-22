# 📊 Customer Marketing Analytics Dashboard (Tableau)

An interactive Tableau dashboard that tells the story of **2,205 customers**: what they buy, where they buy it, how much they earn, and which of them respond to marketing campaigns. Instead of staring at tables, the dashboard answers real questions: **Where does the money come from? Which channel works best? Who responds to campaigns? Does income change spending?**

<img width="1880" height="963" alt="image" src="https://github.com/user-attachments/assets/d44f4075-7568-4d7c-b0f8-5af5093a8722" />


---

## 🗂️ Project Contents

| File | Description |
|---|---|
| `CustomerMarketingDashboard.twb` | The complete Tableau workbook |
| `images/` | Dashboard screenshots |
| `data/` | The dataset (CSV) |

**Data columns used in the report:** Income · Number of Children · Recency · MntWines · MntFruits · MntMeatProducts · MntFishProducts · MntSweetProducts · MntGoldProds · Purchases by Channel (Store / Web / Catalog / Deals) · AcceptedCmp1 to AcceptedCmp5 · Response · Income Tier

---

## ❓ Questions This Dashboard Answers

### KPI Cards: "Where do we stand right now?"

| Card | Value | The Story |
|---|---|---|
| 👥 TotalCustomer | **2,205** | The size of the customer base. |
| 🎯 TotalCampaignPurchases | **333** | Customers who accepted at least one campaign offer. |
| 💰 IncomeAvg | **51,622** | The average customer sits in the middle-income range. |
| 👶 NumberOfChildren | **2,205** | Record count shown on the card (see the note in *Known Issues*). |

> About **15%** of customers (333 / 2,205) accepted a campaign offer, so most of the customer base is still untouched by marketing.

### Charts

| Chart | Question | Short Answer |
|---|---|---|
| Spending by Product Category | What do customers spend on? | Wines dominate by a wide margin, then Meat. |
| Purchases by Channel | Where do customers buy? | Store is the leading channel, then Web. |
| Response Rate by Recency | Does it matter how recently they bought? | Yes. Recent customers respond more. |
| Campaign Response Rate | Which campaigns worked? | The last campaign (Response) is the strongest. |
| Avg. Spending by Income Tier | Do richer customers spend more? | Yes. Higher tiers spend more. |

---

## 🎨 Dashboard Design

A clean, consistent **green theme** keeps the focus on the numbers.

| Role | Color | Where it's used |
|---|---|---|
| KPI cards | Soft pale-green background | Large green values with clear labels |
| Chart titles | Bold green text | Uniform headers on every visual |
| Chart series | Mid green shades | Bars, dots and treemap blocks |
| Page background | Light grey | Lets the cards and charts stand out |

---

## 📄 Dashboard Walkthrough

### 🛍️ Chart 1: Spending by Product Category
**Type:** Horizontal bar chart · **Question:** Which products earn the most?

**The story:** Spending on **MntWines reaches roughly 680K+**, about twice the next category. **MntMeatProducts follows at roughly 360K.** Gold products, Fish, Sweets and Fruits each add a small share (about 60K to 100K each).

> **Takeaway:** Wine and meat are the revenue core. Promotions, bundles and stock planning should start there.

*(Values are read from the chart and are approximate.)*

### 🏬 Chart 2: Purchases by Channel
**Type:** Column chart · **Question:** Where do customers prefer to buy?

**The story:** **Store** is by far the biggest channel (about 20K purchases), followed by **Web** (about 8K). **Catalog** and **Deals** are small.

> **Takeaway:** Physical stores are still the main sales engine, but Web is a solid second. Catalog and Deals contribute little and should be reviewed for cost versus return.

### 📉 Chart 3: Response Rate by Recency
**Type:** Scatter plot with trend line · **Question:** Does recent activity predict response?

**The story:** The trend line **slopes downward**. Customers who bought recently (low recency, near 0 days) respond at higher rates, while response falls steadily as the days since the last purchase grow toward 100.

> **Takeaway:** Contact recent customers first and with the best offers. Long-inactive customers need a different win-back approach, not the same campaign.

### 🎯 Chart 4: Campaign Response Rate
**Type:** Bar chart · **Question:** Which campaigns performed best?

| Campaign | Approx. Acceptance Rate |
|---|---|
| AcceptedCmp1 | ~6% |
| AcceptedCmp2 | ~1% ⚠️ |
| AcceptedCmp3 | ~7% |
| AcceptedCmp4 | ~7% |
| AcceptedCmp5 | ~7% |
| **Response (last campaign)** | **~15% ⭐** |

**The story:** Campaigns 1, 3, 4 and 5 performed similarly at around 6-7%. **Campaign 2 almost failed.** The final campaign more than **doubled** the acceptance rate of all earlier ones.

> **Takeaway:** Something in the last campaign worked far better (offer, timing, channel or targeting). Identify it and repeat it. Find out why Campaign 2 failed so it isn't repeated.

### 💵 Chart 5: Average Spending by Income Tier
**Type:** Treemap · **Question:** Does income change spending?

**The story:** The tiers shown are **Very High (100K+)**, **High (75-100K)** and **Upper-Mid (50-75K)**, plus smaller blocks for lower tiers. The higher the income tier, the darker the block and the higher the average spending.

> **Takeaway:** Income is a strong spending signal. Premium offers (fine wines, gift sets) should be aimed at the High and Very High tiers.

---

## 🧩 The Whole Story in 6 Sentences

1. The business has **2,205 customers** with an average income of about **51.6K**.
2. **Wines and Meat** make up most of the spending.
3. **Store** is the main purchase channel, with **Web** in second place.
4. Only about **15% of customers** accepted a campaign offer.
5. **Recent customers respond more**, and response decays as time since the last purchase grows.
6. **Higher income means higher spending**, and the final campaign was the best performer.

---

## 🧭 Strategic Action Plan

### 🎯 The Core Problem
Marketing reaches many customers but converts few, and spending is concentrated in two categories, one channel and the higher-income groups.

### Strategy 1: Target by Recency 🕐
**Insight:** Response rate falls as recency grows.

| Tactic | How | Metric to Track |
|---|---|---|
| Fast follow-up | Send offers within days of a purchase | Response rate for recency < 30 days |
| Win-back flow | Separate campaign for customers inactive 60+ days | Reactivation rate |
| Recency segments | Build Hot / Warm / Cold lists in the CRM | Response per segment |

### Strategy 2: Repeat What Worked in the Last Campaign 🔁
**Insight:** The last campaign roughly doubled earlier acceptance rates.

| Tactic | How | Metric to Track |
|---|---|---|
| Post-campaign review | Compare offer, channel and audience against earlier campaigns | Acceptance rate |
| Retire weak formats | Drop the Campaign 2 approach | Cost per accepted offer |
| A/B tests | Test one change at a time | Lift vs control |

### Strategy 3: Focus on Wines and Meat 🍷🥩
**Insight:** These two categories carry most of the spending.

| Tactic | How | Metric to Track |
|---|---|---|
| Premium bundles | Wine + meat gift sets | Average basket value |
| Loyalty perks | Early access or subscriptions for top buyers | Repeat purchase rate |
| Grow the small categories | Cross-sell Fruits, Sweets and Fish with wine and meat orders | Share of spend outside Wine and Meat |

### Strategy 4: Strengthen the Right Channels 🏬🌐
**Insight:** Store leads and Web follows. Catalog and Deals are small.

| Tactic | How | Metric to Track |
|---|---|---|
| In-store promotions | Use stores for the best offers and events | Store purchases |
| Grow Web | Online-only offers and easy reorders | Web share of purchases |
| Review Catalog and Deals | Keep only if the return justifies the cost | Profit per channel |

### Strategy 5: Tier Offers by Income 💎
**Insight:** Spending rises with income tier.

| Tactic | How | Metric to Track |
|---|---|---|
| Premium line for High / Very High | Exclusive products and early access | Spend per tier |
| Value bundles for Upper-Mid | Offers that nudge them up in basket size | Movement between tiers |

---

## 🗓️ Implementation Roadmap

| Phase | Timeframe | Focus |
|---|---|---|
| **Phase 1: Quick Wins** | 0-30 days | Recency segments, review the last campaign, pause weak formats |
| **Phase 2: Optimize** | 30-90 days | A/B tests, premium bundles, income-tier offers |
| **Phase 3: Scale** | 90-180 days | Loyalty program, Web growth, channel review |

## 📊 Success KPIs

| KPI | Today | Direction |
|---|---|---|
| Customers who accepted an offer | ~15% (333 / 2,205) | ⬆️ Increase |
| Last campaign acceptance | ~15% | ⬆️ Keep or improve |
| Spending outside Wine and Meat | Small | ⬆️ Increase |
| Web share of purchases | Second channel | ⬆️ Increase |

---------

## 🧰 Tools Used

- **Tableau**: dashboard design and visualizations
- **Calculated fields**: Total Customers · Campaign Purchases · Avg Income · Income Tier · Response Rate
- **Charts**: bar chart, column chart, scatter plot with trend line, treemap
- **Data preparation**: cleaning and tiering of the customer marketing dataset

⭐ If you like this dashboard, leave a star on the repo!
