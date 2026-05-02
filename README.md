# Vanguard A/B Test Analysis

## Overview
This project was developed as part of a statistics and data analytics module. The objective is to analyze a digital A/B test conducted by Vanguard to evaluate whether a redesigned user interface improves the client experience and increases process completion rates.

The experiment compares two groups:
- **Control Group**: Existing interface  
- **Test Group**: Redesigned digital experience  

The main goal is to determine if the new design leads to better performance and usability.

---

## Approach

### Data Sources
- **Client Profiles**: Demographics (age, gender, accounts, balance)
- **Digital Footprints**: User interactions across the process
- **Experiment Roster**: Control vs Test assignment

### Methodology
- Data cleaning, merging, and feature engineering
- Exploratory Data Analysis (EDA)
- KPI definition:
  - Completion Rate
  - Error Rate (backward + skipped steps)
  - Session Duration
  - Digital Engagement (`calls_6_mnth`)
- Hypothesis testing (z-test and t-test)
- Cost-effectiveness validation (minimum +5% improvement)

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
The redesigned interface significantly improves completion rate and meets the cost-effectiveness threshold. However, it introduces higher error rates and longer session durations, indicating usability challenges.

The reduction in help-related calls suggests improved perceived usability.

**Final Verdict: Partially Validated**

---

## Visualization
Interactive dashboards were built in Tableau to:
- Compare Control vs Test performance
- Analyze results by demographics (e.g., age groups)
- Support storytelling and business insights

---

## Tools
- Python (Pandas, NumPy, SciPy)
- Jupyter Notebook
- Tableau

---

## Next Steps
- Improve navigation to reduce errors
- Optimize process efficiency
- Perform deeper segmentation analysis
- Validate findings with user feedback
