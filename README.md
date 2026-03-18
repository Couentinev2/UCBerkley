# Will the Customer Accept the Coupon?

## Summary of Findings

This project explores a dataset of in-vehicle coupon offers collected via Amazon Mechanical Turk. The goal is to identify which driver and contextual characteristics predict whether a coupon will be accepted.

### Overall Acceptance Rate
Approximately **56.8%** of all coupons in the dataset were accepted.

---

### Bar Coupons

**Acceptance rate: ~41%**

Key findings from the bar coupon analysis:

- **Frequent bar visitors accept at much higher rates.** Drivers who visit bars more than 3 times/month accept at ~77%, vs ~37% for those who go 3 or fewer times.
- **Age matters less than habit.** Drivers over 25 who frequent bars have a higher acceptance rate (~69%) compared to all others (~46%).
- **Social context matters.** Drivers without kids and not in farming/fishing/forestry occupations accept at ~71% when they're frequent bar-goers.
- **Young + frequent = most receptive.** Drivers under 30 who go to bars more than once a month are among the most likely to accept.

**Hypothesis:** Bar coupon acceptors are socially active young adults who already frequent bars, are traveling without children, and respond to value-based incentives.

---

### Coffee House Coupons (Independent Investigation)

**Acceptance rate: ~50%** (highest among the coupon types analyzed")

Key findings:

- **Visit frequency is the strongest predictor.** Regular coffee house visitors (1+ times/month) accept at significantly higher rates than non-visitors.
- **Time of day matters.** 10AM and 2PM time slots show the highest acceptance. Aligned with natural coffee-drinking times.
- **Social companions increase acceptance.** Drivers with friends or a partner are more receptive than those alone or with kids.
- **Young adults (21-30) are most receptive.**

**Most receptive profile:** Age 21-30, frequent coffee house visitor, traveling with friends/partner during morning or afternoon.

---

## Notebook

The full analysis is available in [`prompt.ipynb`](prompt.ipynb).

It covers:
1. Data cleaning (missing values, dropped `car` column)
2. Exploratory visualizations (coupon distribution, temperature histogram)
3. Bar coupon deep-dive (7 guided analyses)
4. Independent investigation into Coffee House coupons

## Data Source

UCI Machine Learning Repository: collected via Amazon Mechanical Turk.
