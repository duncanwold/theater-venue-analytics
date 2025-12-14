# Theater Venue Analytics 

> Studies in audience psychology created while running an in-house analytics shop at a live entertainment venue

Hello fellow data enthusiasts! This repository showcases the analytics work I did while operating PianoFight, which was during its time (2014-2023) the most active indy arts venues on the west coast of the United Stages. I ran our in-house "Analytics Shop" to help us better understand our buisness, and our customers.  

These analyses are based on ticketing data retrieved from the Eventbrite API, and were processed using a combination of R, Javascript, and Python for statistical analysis and visualization.

## The Mission

Understand what factors do and don't affect ticket buying decisions in order to...
-  Optimize the weekly programming calendar  
-  Create marketing and pricing "best practices" for show producers 
-  Spend our time focused on what actually matters

**Spoiler alert:** The results often challenged what I expected to find going in to each case study.

## Case Studies

### [Do higher priced tickets drive down demand?](./case-study-1-pricing-demand/)

**Initial Assumption:** Yes. As ticket prices increase, demand will fall.

**Surprising Result:** We found a *positive* relationship between ticket price and tickets sold.

**Business Impact:** Helped producers feel confident that they could charge the price their budget required, without losing audience.

**Key Insight:** Price is a signal of quality. A $25 show is perceived as higher quality than a $5 show.

---

### [What are the most valuable show start times in our weekly calendar?](./case-study-2-optimal-showtimes/)

**Initial Assumption:** Weekend primetime shows would sell best.

**Surprising Result:** When we normalized by *number of shows* instead of *calendar weeks*, mid-week and late-night slots performed nearly as well.

**Business Impact:** Shifted programming strategy to fill underutilized time slots, increasing total venue revenue by maximizing all available inventory. Note: This was by far the *most* impactful case study we worked on at PianoFight. It really transformed a big part of our buisness.

---

### [Do higher ticket prices correlate to higher bar sales?](./case-study-3-bar-sales-correlation/)

**Initial Assumption:** Customers who buy higher priced tickets will also spend more on food and drink than those spending less.

**Surprising Result:** We found *no* correclation between the price of a show and the per person spend at the bar.

**Key Insight:** Customers evaluate entertainment purchases differently than food/drink purchases. Price sensitivity varies by purchase category.

## Methodology

### Data Collection
- **Source:** Eventbrite API, Door counts collected on site
- **Scope:** 3+ years of ticketing data (2016-2019)
- **Volume:** Thousands of events, tens of thousands of transactions
- **Automation:** [Revenue Wizard](https://github.com/duncanwold/revenue-wizard) tool for data extraction

### Analysis Tools
- **R** for statistical analysis and visualization
- **Linear regression** for correlation analysis
- **Heatmap visualizations** for time-series patterns
- **ggplot2** for publication-quality graphics

### Key Techniques
- Regression analysis (price vs demand)
- Multi-dimensional aggregation (day × time × revenue)
- Normalization strategies (per-week vs per-show)

## Repository Structure

Each case study includes:
- `README.md` - Full analysis write-up
- Visualizations (PNG files)

## Related Projects

This analytics work was enabled by the [Revenue Wizard](https://github.com/duncanwold/revenue-wizard), an automated financial reconciliation and buisness analytics tool that I built.

## Background on PianoFight

PianoFight was a venue in San Francisco with three event spaces, which ran aroun 25-30 shows per week (over 9000 in total). The programming was extremely ecclectic: comedy, theater, concerts, film, drag, dance, game shows, etc. I shared these insights with Eventbrite's data team in 2020 (where I curretnly work) as examples of how venue operators can leverage ticketing data.

## Questions?

Have questions about the methodology? Want to discuss venue analytics? 

Feel free to open an issue or reach out!
