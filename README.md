# social-media-analytics-portfolio
Data analysis of LinkedIn &amp; Twitter performance for a food-tech startup. Uncovered key insights including 57% negative hashtag impact and delivered actionable recommendations using Python and Power BI.

# 📊 Social Media Performance Analysis: Data-Driven Growth Strategy

## Project Overview

**Duration:** 2 weeks (January 2026)  
**Role:** Data Analyst  
**Tools:** Python (pandas, matplotlib, seaborn), Jupyter Notebook, Power BI, Buffer Analytics

---

## 🎯 Business Context

An early-stage food-tech startup providing a platform for local restaurants and food businesses needed data-driven insights to optimize their social media strategy. After one month of consistent posting on LinkedIn and Twitter, the company lacked visibility into what content was working and how to allocate resources effectively.

## 📈 Key Results

### LinkedIn
- ✅ **75% follower growth** in 30 days (116 → 203 followers)
- ⚠️ **Identified declining momentum:** -12.9% in second half of month
- 📍 **Pinpointed success formula:** Week 3 performance (+27 followers) and peak day analysis (Jan 11: +13 followers)

### Twitter
- ✅ **12.19% engagement rate** (12x industry average of 0.5-1%)
- 🔴 **Critical issue discovered:** Average 67.5 impressions/post severely limiting reach
- 💡 **Key insight:** Hashtag strategy backfiring (posts without hashtags performed 57% better)

## 🔍 Analysis Approach

### Data Collection
- **Source:** Buffer social media management platform (CSV exports)
- **LinkedIn:** 30 days of daily follower counts (Jan 2-31)
- **Twitter:** 15 posts with full engagement metrics (Jan 1-28)

### Methodology

**1. Data Preparation**
```python
# Sample code structure
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load and clean data
linkedin_df = pd.read_csv('Downoloads/linkedin_metrics.csv')
twitter_df = pd.read_csv('Downloads/twitter_metrics.csv')

# Feature engineering
linkedin_df['Daily Change'] = linkedin_df['Total Followers'].diff()
linkedin_df['7-Day Rolling Avg'] = linkedin_df['Daily Change'].rolling(window=7).mean()
twitter_df['engagement_rate'] = (twitter_df['engagement'] / twitter_df['impressions']) * 100
```

**2. Statistical Analysis**
- Descriptive statistics (mean, median, std deviation)
- Cohort analysis (first-half vs second-half comparison)
- Outlier detection for high-growth days (mean + 1 std deviation)
- Trend identification using rolling averages

**3. Content Performance Analysis**
- Regex pattern matching to classify content themes
- Hashtag count analysis and performance correlation
- Series content tracking ("Gamify Your Life" case study)

## 💡 Key Insights Discovered

### LinkedIn Findings
1. **Strong overall growth** but momentum declining (3.21/day → 2.80/day → 1.86/day last week)
2. **High-growth days identified:** 4 days exceeded 6+ followers (Jan 10, 11, 16, 22)
3. **Plateau pattern:** 7 days (23% of month) with zero growth
4. **Best performing week:** Week 3 with 27 new followers

### Twitter Findings
1. **Exceptional engagement quality** but critically limited reach
2. **Hashtag strategy failing:** Posts without hashtags: 16.6% engagement vs with hashtags: 10.6% (-57% impact)
3. **Series content wins:** "Gamify Your Life" series averaged 33.3% engagement
4. **Educational content resonates:** Fasting/health posts: 13.5% avg engagement

## 📊 Visualizations Created

### Python Dashboards (matplotlib/seaborn)
- 4-panel LinkedIn growth analysis
- Daily follower change with rolling averages
- Growth rate percentage trends
- Distribution histograms

### Power BI Dashboard
- Executive KPI cards
- Platform comparison views
- Interactive filters by date, content theme
- Goal tracking gauges

## 🎯 Strategic Recommendations Delivered

### Priority 1: LinkedIn Momentum Recovery
- Content audit of Week 3 and Jan 11 success
- Implement daily engagement protocol (10-15 accounts)
- Increase posting frequency to 4-5x/week
- **Target:** Restore to 3+ followers/day

### Priority 2: Twitter Reach Expansion
- Eliminate hashtag overuse (max 1-2 per post)
- Create 2-3 new series content formats
- Daily influencer engagement strategy
- **Target:** Increase avg impressions from 67.5 to 200+

### Priority 3: Content Strategy Framework
- 40% Thought leadership
- 30% Educational content
- 20% Behind-the-scenes
- 10% Industry news commentary

## 📈 Expected Business Impact

| Metric | Current | 30-Day Target | Improvement |
|--------|---------|---------------|-------------|
| LinkedIn Daily Growth | 1.86/day | 3.0+/day | +61% |
| LinkedIn Total Followers | 203 | 285 | +40% |
| Twitter Avg Impressions | 67.5 | 200+ | +196% |
| Twitter Engagement Rate | 12.19% | Maintain >10% | Sustained excellence |

## 🛠️ Technical Skills Demonstrated

### Data Analysis
- Python data wrangling (pandas)
- Statistical analysis & trend identification
- Feature engineering & data transformation
- Time-series analysis

### Visualization
- Multi-panel dashboards (matplotlib, seaborn)
- Interactive business intelligence (Power BI)
- Effective visual storytelling

### Business Acumen
- Stakeholder communication (CEO, marketing team)
- Strategic recommendation development
- ROI-focused insights
- Problem diagnosis & solution design

## 📁 Repository Structure

```
social-media-analysis/
├── data/
│   ├── linkedin_metrics.csv
│   └── twitter_metrics.csv
├── notebooks/
│   ├── 01_linkedin_analysis.ipynb
│   ├── 02_twitter_analysis.ipynb
│   └── 03_combined_insights.ipynb
├── dashboards/
│   ├── power_bi_dashboard.pbix
│   └── dashboard_screenshots/
├── reports/
│   ├── executive_summary.pdf
│   └── detailed_analysis.docx
├── visualizations/
│   ├── linkedin_growth_analysis.png
│   └── twitter_engagement_breakdown.png
└── README.md
```

## 🎓 Key Learnings

1. **Counterintuitive insights matter:** The hashtag analysis revealed that conventional wisdom (more hashtags = better reach) was actually hurting performance
2. **Momentum is fragile:** Even with strong overall growth, declining trends need immediate attention
3. **Content quality ≠ Reach:** Twitter's exceptional engagement was meaningless with only 67.5 avg impressions
4. **Series content creates anticipation:** Serialized posts (Gamify series) drove 2.2x better engagement

## 📞 Project Outcome

**CEO and marketing team approved implementation of all recommendations.** The analysis transformed the company's social media approach from intuition-based to evidence-based decision making.

---

## 📫 Contact & Portfolio

**LinkedIn:** www.linkedin.com/in/babatope-bakare 
**Email:** bakaret74@gmail.com

---

*This project demonstrates my ability to extract actionable business value from raw data, communicate complex findings to non-technical stakeholders, and drive strategic decision-making through analytics.*

