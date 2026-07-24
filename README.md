# Vanguard Digital Redesign: A/B Test Analysis

## 📌 Project Overview

Vanguard evaluated a redesigned User Interface (UI) featuring in-context prompts against its traditional interface. The primary goal was to determine whether the updated design meaningfully improves process completion rates among clients.

- **Experiment Period:** March 15 – June 20, 2017
- **Target Audience:** Established Vanguard client base (Median age: 47.3 years | Median tenure: 11 years)
- **Core Question:** Would the redesigned UI encourage more clients to complete the process without introducing excessive friction?

**Presentation:** [View on Canva](https://canva.link/44rhlfr9flm13dl)

**Repo:** [mocihu-source/Week-5-6-Project--EDA-and-Inferential-Stats](https://github.com/mocihu-source/Week-5-6-Project--EDA-and-Inferential-Stats/tree/main)

## 👥 Team Members

Presented by the Data Analytics Team:

- Katarzyna
- Moci
- Keagan
- Teresa

## 📊 Dataset & Cleaning Steps

- **Data Sources:** Merged three core datasets — client demographics, web interaction logs, and the experiment roster. Each client was mapped via a unique client ID.
- **Data Volume:** Cleaned ~755,000 raw web events down to 68,941 visits across 50,487 unique clients. Out-of-scope and incomplete records were removed.
- **Data Quality Fixes:** Corrected duplicate logging events and visit ID collisions.
- **Randomization Validation:** Baseline engagement (e.g., average 6-month logins ~6.1 and support calls ~3.1) was balanced across both groups, confirming valid randomization.

## 📈 Key Metrics & Results (KPIs)

| Metric | Control UI | Test UI | Delta / Impact | Significance |
|---|---|---|---|---|
| Completion Rate | 49.6% | 58.4% | +8.7 pp (~17% relative lift) | p < 0.0001 (z = 22.89) |
| Median Completion Time | 4.57 min | 4.18 min | −0.39 min (~8.5% faster overall) | p < 0.0001 (Mann-Whitney U) |
| Avg. Support Calls (6 mos) | 3.13 | 3.06 | −0.07 calls | p < 0.001 (small practical impact) |

### Key Behavioral Insights

- **Funnel Performance:** Test group drop-off was significantly reduced at two of the four funnel transitions (p < 0.001), with the strongest improvements at the start and final stages.
- **Error Rate & In-Context Prompts:** Test UI users showed higher error/backward-navigation rates early in the funnel (Start, Step 1, Step 2, and Confirm). However, overall completion rates improved, indicating the UI trades some speed for added guidance.
- **Critical Friction Point:** Drop-offs peaked at the Step 2 → Step 3 transition, suggesting early step confusion that occasionally culminates in abandonment later.

## 💡 Conclusions & Recommendations

- **Proceed with Full Rollout:** The test UI achieved an +8.7 percentage point increase in completion rate, comfortably exceeding Vanguard's 5 percentage point threshold.
- **Optimize Step 2 → Step 3 Transition:** Address user confusion in the early steps (Steps 1–2) to prevent mid-funnel drop-offs.
- **Post-Rollout Qualitative Survey:** Deploy targeted user satisfaction surveys to monitor user sentiment regarding error frequency.

## ⚠️ Limitations & Data Needed

- **Seasonality:** The experiment period (Mar–Jun 2017) overlapped with the US tax season, which may skew client behavior.
- **Missing Data Points:** Granular call timing data, device/platform breakdowns, and direct qualitative user feedback were unavailable.

## 🛠 Tech Stack

- **Language:** Python (Pandas, NumPy, SciPy, Statsmodels)
- **Visualization:** Tableau (Demographic & Engagement Dashboards), Seaborn, Matplotlib
- **Version Control:** Git & GitHub
