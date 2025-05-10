# Impact of NIL Policy on Basketball Student-Athletes
## Overview
This project investigates the impact of the NIL (Name, Image, and Likeness) policy on NCAA basketball student-athletes, using a combination of Difference-in-Differences (DiD) analysis, exploratory data analysis (EDA), and a predictive machine learning model -- Random Forest.

The project also provides practical insights for stakeholders including UMN (University of Minnesota) and NIL Business Development Agency, aiming to identify high-potential talent for NIL deals and uncover strategies to support athlete success both on and off the court.

---

## Key Research Questions
- Did the NIL policy influence student-athletes' on-court performance?
- What kind of players are more likely to receive NIL deals?
- What actions can UMN & agency take to support more deals for their players?

---

## Dataset
- NIL Deals: Web-scraped from [NCAA Name, Image, and Likeness News & Data](nilcollegeathletes.com)
- Clients Provided Performance Data: Includes pre- and post-NIL stats such as:
-- Points, rebounds, assists, steals, blocks, turnovers
-- WS.40, OWS, DWS (Win Share metrics)
-- Minutes played, fouls, field goal attempts/made

---

## Methodology
### Difference-in-Differences (DiD) Analysis
**Goal:** Isolate the causal effect of NIL policy on player performance.
**Metric Used:** WS.40 (Win Shares per 40 minutes)
**Design:**
- U.S. players = treatment group (NIL policy implemented)
- Canadian players = control group (no NIL policy)
**Result:** NIL policy is associated with performance increases of:
- +0.0161 for male athletes
- +0.0085 for female athletes
DiD Analysis controlled for fixed player-specific characteristics (like talent, position, playing style) to estimate the treatment effect more accurately.

### Predictive Modeling (Random Forest)
**Goal:** Predict which players are more likely to secure NIL deals.
**Model:** Random Forest Classifier
**Performance:** AUC = 0.80
**Key Predictors:**
- Shooting metrics (FGA, FTA, 3PTA)
- Minutes played, personal fouls, win shares
**Outcome:** A ranked list of high-potential athletes who haven't yet received deals.

### Benchmarking Resources
Compared UMN with peer institutions receiving 4–6 NIL deals.
**Identified gaps in:** 
- Legal/contract support
- Entrepreneurship/NIL-related curriculum
- Brand partnerships
**Recommended building:**
- NIL course with Carlson School of Management
- National brand activation support
- Formalized NIL support structure for athletes

---

## Key Findings
- Both deal and non-deal players improved after NIL introduction, but deal recipients saw greater gains. WS.40 increased for both men (+13.5%) and women (+12.7%) after NIL.
- Players with strong shooting stats and efficiency are more likely to secure NIL deals.
- UMN is mid-tier in deal count, with strengths in alumni/media support, but opportunities to improve on legal and academic support.

---

## Future Work
- Enhance predictive model by integrating social media visibility and off-court influence features.
- Apply Synthetic Control Method to validate robustness when DiD assumptions may not hold.
- Expand analysis to other sports or divisions for broader insights.
