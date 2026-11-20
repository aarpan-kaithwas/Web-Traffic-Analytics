# Web Traffic & User Engagement Analysis

Exploratory data analysis of 2,000 website sessions (`website_wata.csv`) examining visitor behavior, acquisition channel performance, and engagement drop-offs across the user journey.

## Files Included
- `web_traffic_analysis.ipynb` — Jupyter Notebook containing data validation, channel segmentation, funnel drop-off mapping, and visualizations.
- `website_wata.csv` — Session-level web traffic dataset (2,000 records across 7 metrics).
- `traffic_analysis_charts.png` — Summary grid of traffic volume, bounce rates, user funnel progression, and metric correlations.

## Key Findings
- **Session Overview:** Users average **4.95 page views** and **3.02 minutes** per session, with an overall average bounce rate of **28.5%**.
- **Acquisition Channels:** **Organic** search drives the largest traffic share (786 sessions, 39.3%), while **Referral** traffic delivers the lowest bounce rate (26.6%) and longest average session duration (3.13 mins). **Social** traffic shows the highest bounce rate (29.6%) and lowest page depth (4.70).
- **Visitor Retention:** Returning visitors represent **85.9%** of sessions (1,718 vs. 282 new visitors) and convert slightly higher (98.4% vs. 96.8%).
- **Primary Drop-Off Point:** While 95.9% of visitors view at least two pages, **40.3%** drop off before reaching 1.5 minutes of engagement (593 sessions last under 1 minute).
- **Conversion Drivers:** `Time on Page` (r = 0.23) and `Session Duration` (r = 0.18) correlate most strongly with conversion rate.

## Actionable Recommendations
1. **Improve early landing-page retention:** Strengthen above-the-fold clarity and internal links to convert sub-minute browsers into engaged multi-minute sessions.
2. **Align Social landing pages with campaign copy:** Reduce the 29.6% bounce rate on Social traffic by matching post messaging closely to destination pages.
3. **Fix tracking tag misfires:** Audit the 14 sessions that recorded active duration with `0` page views.
