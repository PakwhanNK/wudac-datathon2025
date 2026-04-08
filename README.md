# eBay User Segmentation & Conversion Analysis

A datathon project that segments eBay users into behavioral personas and identifies what drives purchases — turning raw marketplace data into actionable business strategy.

---

## The Problem

> How can we segment eBay users into meaningful behavioral personas, and what drives conversion on the platform?

eBay's mix of new and second-hand goods creates a uniquely diverse user base, where standard e-commerce analytics may miss the nuance. For example, value hunters, collectors, and family shoppers all behave very differently. Therefore, we would like to investigate more on how many user groups we can classify, and how eBay should respond to these.

---

## Dataset

| Dataset | Records |
|---|---|
| Unique users | 101,426 |
| Successful transactions | 147,947 |
| Unique sessions | 2,771,371 |

Built from three sources: `sessions.csv`, `transactions.csv`, and `product_categories.csv`, filtered to eBay users and merged into user-level and session-level datasets.

---

## Approach

**1. K-Means Clustering** — grouped users into 4 personas based on browsing patterns, demographics, and purchase behavior (cluster count selected via scree plot).

**2. Logistic Regression** — one model per cluster to identify which features most strongly predict conversion within each segment.

---

## Key Findings

| Persona | Share | Profile |
|---|---|---|
| Homeowners / couples | 27% | Practical shoppers; home, auto, beauty |
| Lifestyle & hobby shoppers | 49% | Largest segment; discovery-driven |
| Value-conscious families | 8% | Budget-aware; respond to savings messaging |
| Younger families with children | 17% | Household-driven; children's presence is a strong conversion signal |

**Top business takeaways:**
- Household composition (especially children) is one of the strongest conversion predictors
- The largest segment responds to personalized, interest-based recommendations
- Budget segments convert on discounts, bundles, and retargeting

---

## Deliverables

- [`reports/WUDAC Report Non-tech.pdf`](reports/WUDAC%20Report%20Non-tech.pdf) — executive summary for business stakeholders
- [`reports/WUDAC Report Tech.pdf`](reports/WUDAC%20Report%20Tech.pdf) — full technical walkthrough

