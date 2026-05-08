# Vanguard A/B Test Analysis

## Overview
This project was developed as part of a statistics and data analytics module. The objective is to analyze a digital A/B test conducted by Vanguard to evaluate whether a redesigned user interface improves the client experience and improves process completion rate.

The experiment compares two groups:
- **Control Group**: Existing interface (23,435 users)  
- **Test Group**: Redesigned digital experience (26,866 users)  

The main goal is to determine if the new design leads to better performance and usability.

---

## Approach

### Data Sources
- **Client Profiles**: Demographics (age, gender, accounts, clients' tenure)
- **Digital Footprints**: User interactions across the process
- **Experiment Roster**: Control vs Test assignment

### Methodology
- Data cleaning, merging, and feature engineering
- Exploratory Data Analysis (EDA)
- KPI definition:
  - Completion Rate
  - Error Rate (backward + skipped steps)
  - Session Duration (for the completed and non-completed sessions)
  - Digital Engagement (`calls_6_mnth`)
- Hypothesis testing (z-test and t-test)
- Cost-effectiveness validation (minimum +5% improvement in Completion rate)

---

## Key Results

| Metric           |Control | Test   | Outcome |
|------------------|--------|--------|---------|
| Completion Rate  | 49.7%  | 58.4%  | +17.5% Completion rate Improved   |
| Error Rate       | 7.09%  | 9.66%  | 2.5pp Error Rate Increased (+8pp for the first step) |
| Session Duration | 6.54min| 6.00min| 8.1% Improved Duration for the Completed sessions  |
| Calls (6 months) | 3.13   | 3.06   | 2.2% Fewer help requests per client |

---

## Conclusion
- The redesigned interface significantly improves Completion rate and exeeds the cost-effectiveness threshold of 5% - with 17.5% improvement for the Test group. 
- However, it introduces higher Error rate especially for completing the first step. 
- Session duration for the Test, indicating 8.1% fester process for the completed sessions.
- A number of help-related calls per user was slightly improved by 2.2%, which suggests improved perceived usability.

**Final Verdict: Partially Validated**

---

## Visualization
Interactive dashboards were built in Tableau to:
- Compare Control vs Test performance
- Analyze results by demographics (e.g., age groups, gender, tenure)
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

Link to the presentation: https://docs.google.com/presentation/d/1JI7WQgXP3nGbdGpRa-cR-DSqZVQ59Qeb/edit?usp=sharing&ouid=111978843608016953666&rtpof=true&sd=true
