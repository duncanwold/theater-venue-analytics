# Theater Venue Analytics 

> Data-driven insights from running an in-house analytics shop at a live entertainment venue

Welcome fellow data enthusiasts! This repository showcases analytics work I did while operating PianoFight, a theater and bar venue in San Francisco. I built an in-house "Venue Analytics Shop" to understand our business better and (hopefully) make more money 💰

All analyses are based on ticketing data retrieved from the Eventbrite API, processed using R for statistical analysis and visualization.

## The Mission

Transform gut-feeling venue management into data-driven decision making by:
-  Testing assumptions about pricing and demand
-  Optimizing the weekly programming calendar  
-  Understanding customer behavior patterns
-  Maximizing revenue across all channels

**Spoiler alert:** The data frequently contradicted conventional wisdom in the entertainment industry.

## Case Studies

### [Do higher priced tickets drive down demand?](./case-study-1-pricing-demand/)

**Surprising Result:** NO! We found a *positive* relationship between ticket price and tickets sold.

**Business Impact:** Convinced producers they could raise prices without losing audience, allowing us to increase rental rates while producers passed costs to buyers.

**Key Insight:** Price signals quality. A $25 show is perceived as higher quality than a $5 show.

---

### [What are the most valuable show start times in our weekly calendar?](./case-study-2-optimal-showtimes/)

**Initial Finding:** Friday 8PM = 💰💰💰 (Obviously, right?)

**Plot Twist:** When we normalized by *number of shows* instead of *weeks*, mid-week and late-night slots performed nearly as well!

**Business Impact:** Shifted programming strategy to fill underutilized time slots, increasing total venue revenue by maximizing all available inventory.

**Strategic Shift:** Stopped overvaluing Friday/Saturday 8PM and started actively promoting Wednesday comedy and Saturday 10PM late shows.

---

### [Do higher ticket prices correlate to higher bar sales?](./case-study-3-bar-sales-correlation/)

**Hypothesis:** Customers spending $30 on tickets will spend more at the bar than those spending $10.

**Surprising Result:** Actually, not really! Big ticket spenders averaged about the same bar sales per person as budget ticket buyers.

**Key Insight:** Customers evaluate entertainment purchases differently than food/drink purchases. Price sensitivity varies by purchase category.

**Implication:** Don't underestimate the value of lower-priced shows—they drive equivalent bar revenue while filling seats.

## Methodology

### Data Collection
- **Source:** Eventbrite API
- **Scope:** 3+ years of ticketing data (2016-2019)
- **Volume:** Thousands of events, tens of thousands of transactions
- **Automated:** [Revenue Wizard](https://github.com/duncanwold/revenue-wizard) tool for data extraction

### Analysis Tools
- **R** for statistical analysis and visualization
- **Linear regression** for correlation analysis
- **Heatmap visualizations** for time-series patterns
- **ggplot2** for publication-quality graphics

### Key Techniques
- Regression analysis (price vs demand)
- Multi-dimensional aggregation (day × time × revenue)
- Normalization strategies (per-week vs per-show)
- Longitudinal comparison (2016 vs 2018)

## Business Outcomes

These insights weren't just academic exercises—they drove real operational changes:

✅ **Pricing Strategy Overhaul**
- Increased average ticket prices by ~25%
- No decrease in attendance
- Higher revenue per show

✅ **Calendar Optimization**  
- Redistributed shows from "prime time" to underutilized slots
- Increased total weekly revenue
- Better inventory utilization

✅ **Revenue Forecasting**
- More accurate projections
- Better cash flow planning
- Informed programming decisions

## Technical Skills Demonstrated

-  **Statistical Analysis** - Regression, correlation, hypothesis testing
-  **Data Visualization** - Heatmaps, scatter plots, trend analysis  
-  **ETL Pipelines** - API data extraction and transformation
-  **Business Analytics** - Translating data into strategy
-  **A/B Validation** - Testing hypotheses with real-world changes
-  **Data Communication** - Making insights accessible to non-technical stakeholders

## Lessons Learned

** Question Your Assumptions**
The most valuable insights came from testing "obvious" industry wisdom that turned out to be wrong.

** Choose Your Metrics Carefully**  
How you normalize data (per-week vs per-show) dramatically changes what you see. Always ask "what am I actually measuring?"

** Close the Loop**
The 2018 heatmap validating our 2016 strategy changes showed the value of implementing insights and measuring results.

** Industry Context Matters**
Live entertainment has unique economics—lessons here might not apply to e-commerce or SaaS, but the analytical approach does.

## Repository Structure

Each case study includes:
- `README.md` - Full analysis write-up
- Visualizations (PNG files)
- R scripts (where available)
- Sample anonymized data (where possible)

## Related Projects

This analytics work was enabled by the [Revenue Wizard](https://github.com/duncanwold/revenue-wizard), an automated financial reconciliation tool I built that:
- Pulled data from Eventbrite API
- Calculated complex revenue splits
- Generated these datasets for analysis

## Background

This work was performed 2016-2019 while operating PianoFight in San Francisco. The venue hosted 500+ shows annually across comedy, theater, music, and film. I shared these insights with Eventbrite's data team in 2020 (where I later worked) as examples of how venue operators can leverage ticketing data.

## Questions?

Have questions about the methodology? Curious about how we implemented changes? Want to discuss venue analytics?

Feel free to open an issue or reach out!

---

*Built with R, curiosity, and skepticism about "the way it's always been done"*
