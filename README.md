# Vanguard A/B Test Analysis

## Overview
This project analyzes the impact of a redesigned digital interface for Vanguard using an A/B testing framework. The objective is to determine whether the new design improves user performance, efficiency, and overall experience compared to the existing interface.

---

## Approach
- **Data Cleaning & EDA**: Prepared and merged datasets, created key features (`age_group`, `session_duration`, `completed`)
- **KPIs Defined**:
  - Completion Rate
  - Error Rate (backward + skipped steps)
  - Session Duration
  - Digital Engagement (`calls_6_mnth`)
- **Hypothesis Testing**:
  - Statistical tests (z-test, t-test)
  - Cost-effectiveness threshold (≥ 5%)

---

## Key Results

| Metric            | Control | Test | Outcome |
|------------------|--------|------|--------|
| Completion Rate  | 49.76% | 58.48% | +8.72pp (significant) |
| Error Rate       | 7.09%  | 9.66%  | Increased |
| Session Duration | 187.7s | 195.9s | Slower |
| Calls (6 months) | 3.13   | 3.06   | Fewer help requests |

---

## Conclusion
The redesign improves completion rate significantly but introduces usability trade-offs, including higher error rates and longer session times.  
The reduction in help-related calls suggests improved perceived usability.

**Final Verdict: Partially Validated**

---

## Visualization
- Built interactive dashboards in Tableau
- Explored results by variation and demographics (age groups)
- Designed story-driven insights for decision-making

---

## Tools
Python (Pandas, SciPy), Jupyter, Tableau

---

## Next Steps
- Reduce friction in key steps
- Improve efficiency (time and errors)
- Refine UX before full rollout
