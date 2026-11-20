# Did New Gamification Features Increase Engagement? (Excel, Statistics)

**Business question:** In 2022 an e-learning platform launched XP points, coins, leaderboards, streaks and a larger course library. Did users engage more in Q4 2022 than in Q4 2021, and does the answer differ for **free vs. paid** users and by **market (US vs. India)**?

**Stack:** Excel · descriptive statistics · skewness/kurtosis · 95 % confidence intervals · Welch two-sample t-tests
**Engagement KPI:** minutes watched per user per quarter

---

## Executive summary

| Segment | Q4 2021 mean | Q4 2022 mean | Change | Test result (α = 0.05, one-sided) |
|---|---|---|---|---|
| **Paid users** | 332.5 min (n = 3,433) | 368.4 min (n = 5,104) | **+10.8 %** | t = −3.05, df = 8,229 → **significant increase** |
| **Free users** | 133.9 min (n = 32,171) | 69.1 min (n = 120,658) | **−48.4 %** | t = 29.78, df = 40,836 → no increase (mean fell) |
| **Free users, US vs. India (2022)** | US 73.1 min | India 78.4 min | – | t = −1.21, df = 11,001 → **no significant difference** |

95 % confidence intervals for the mean: Paid 2021 [316.2, 348.8] vs. 2022 [352.0, 384.7] · Free 2021 [129.9, 137.9] vs. 2022 [67.7, 70.6]. The intervals do not overlap in either segment.

## Interpretation

1. **Paid users engage more after the launch.** The increase is statistically significant and practically relevant (+36 minutes per user per quarter).
2. **The drop in the free-user average is mostly a mix effect, not proof that the features failed.** The free user base grew **3.75x** (32k → 121k). A large number of new, low-intent sign-ups lowers the average. To isolate the effect of the features, the next step is to compare **the same users over time** (cohort view) or **new users by sign-up quarter**.
3. **The data supports correlation, not cause and effect.** There was no control group, so the change cannot be fully attributed to the new features. Seasonality, marketing and content growth changed at the same time.
4. **The distributions are very right-skewed** (2022 skewness up to 15, kurtosis > 300 for free users). A few power users drive the means. Medians and percentile-based KPIs should be reported next to averages. In the 1–100 minute subgroup (Task 1), the **paid median rose from 26 to 40 minutes**, while the **free median fell from 14.2 to 11.8 minutes**.
5. **The US and India behave the same way** among free users. Market strategy can be decided on market size and monetisation, not engagement differences.

## Recommendations

- Measure feature impact with an **A/B test or staggered rollout** next time, using a holdout group.
- Track engagement **per acquisition cohort** and use the **median and share of active users** in addition to the mean.
- Use gamification as a **paid-retention lever**. For free users, focus on activation (first lesson completed, D7 return) before engagement depth.

## Project tasks

| Task | Content |
|---|---|
| 1–2 | Mean, median, mode, SD, skewness and kurtosis for users with 1–100 min in Q4 2021, by plan type |
| 3 | 95 % z-confidence intervals for mean minutes watched, 2021 vs. 2022, free vs. paid |
| 4 | One-sided Welch t-tests, H₀: μ₂₀₂₁ ≥ μ₂₀₂₂. Discussion of Type I and Type II error costs |
| 5 | One-sided Welch t-test, free users US vs. India 2022, H₀: μ_US ≥ μ_IN |

## Files

| File | Content |
|---|---|
| [`data.xlsx`](data.xlsx) | Original anonymised dataset (student_id, country, paid flag, minutes watched Q4 2021/2022) |
| [`Engagement_Project.xlsx`](Engagement_Project.xlsx) | All calculations, one sheet per task |

*Dataset: 365 Data Science, used as a guided case study. The interpretation and recommendations are my own.*
