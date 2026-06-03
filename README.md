# task-07
# TASK 7 — AI Tool Adoption Trend Analysis

## Problem Statement
Analyze AI tool adoption patterns across 500 organizations to uncover trends,
correlations, and segment-level insights that guide AI investment decisions.

## Dataset Description
- **Source:** Synthetic survey dataset (500 organizations)
- **Features:** Industry, AI tool, company size, employee count, adoption year,
  investment, productivity gain, satisfaction score, cost savings, adoption rate
- **Target variables:** adoption_rate_pct, productivity_gain_pct

## Trend Analysis
| Finding | Value |
|---|---|
| Fastest growing period | 2023–2024 (61% of all adoptions) |
| Top AI tool | ChatGPT (31.6% share) |
| Leading industry | Technology (avg 65% adoption) |
| Company size effect | Enterprise 8–12pp above Small |

## Statistical Findings
- **ANOVA:** F=15.21, p≈0 → Company size significantly impacts adoption
- **Pearson r (Adoption↔Productivity):** r=0.29, p<0.0001 (positive, significant)
- **Pearson r (Size↔Adoption):** r=0.29, p<0.0001
- **Mean productivity gain:** 37.7% | **Median adoption rate:** 63.2%

## Visual Insights
- fig1: Tool popularity + industry distribution
- fig2: Descriptive stat distributions
- fig3: Trend investigation (4 charts)
- fig4: Heatmap industry×tool + scatter
- fig5: Correlation matrix
- fig6: Hypothesis testing (ANOVA)
- fig7: Segmentation pie + bar
- fig8: ROI & productivity scatter

## Recommendations
1. SMBs → Start with ChatGPT/Copilot (lowest barrier, proven ROI)
2. Enterprises → Invest in DataRobot / Azure OpenAI for scale automation
3. Healthcare & Logistics → Highest untapped potential; target for growth
4. All orgs → Formalize AI strategy documents (+15% adoption boost)
5. Minimum $20K/yr AI budget for meaningful productivity gains

## Segmentation Summary
| Segment | Count | Avg Adoption | Avg Productivity |
|---|---|---|---|
| AI Leader | 79 | 85.5% | 48.8% |
| Early Adopter | 57 | 69.4% | 35.3% |
| High ROI | 109 | 58.7% | 34.8% |
| High Satisfaction | 73 | 55.2% | 36.6% |
| Mainstream | 165 | 58.7% | 35.7% |
| Slow Adopter | 17 | 27.4% | 36.6% |

## Future Scope
- Time-series forecasting of adoption rates to 2027
- NLP sentiment analysis on AI satisfaction open-text responses
- Predictive model: classify orgs likely to become AI Leaders
- Region-wise analysis for geo-targeting recommendations

## Repository Structure
```
TASK_07_AI_Tool_Adoption_Trend_Analysis/
├── data/         ai_adoption_dataset.csv
├── notebook/     TASK07_AI_Adoption_Analysis.py
├── images/       fig1–fig8 (8 charts)
├── reports/      (PDF report)
├── src/          analysis.py
├── README.md
└── requirements.txt
```

## Requirements
```
pandas numpy matplotlib seaborn scipy scikit-learn
```
