# UC_berkeley_Projects_assi5
This repo contains the code for the practical application5
By Sasan shadpour


Findings:

# Coupon Acceptance Analysis

## Overview

This project analyzes driving coupon acceptance patterns using data from the UCI Machine Learning repository. The analysis explores what factors influence whether drivers accept coupons for different venues through visualizations and statistical summaries.

## Dataset

The dataset contains survey responses describing different driving scenarios including:
- **User attributes**: Gender, age, marital status, income, education, occupation
- **Contextual attributes**: Driving destination, weather, temperature, time, passenger type
- **Coupon attributes**: Coupon type, expiration time

**Coupon Types**: 
- Less expensive restaurants (under $20)
- Coffee houses
- Carry out & take away
- Bars
- More expensive restaurants ($20-$50)

## Key Findings

### Bar Coupon Analysis

**Overall Acceptance Rate**: 41% of bar coupons were accepted.

#### Drivers Most Likely to Accept Bar Coupons:

1. **Frequency of Bar Visits** ✓
   - Drivers visiting bars more than 3 times per month have significantly higher acceptance rates
   - Clear indicator of restaurant/bar interest

2. **Age Factor** ✓
   - Younger drivers (under 30) show higher acceptance rates
   - Drivers under 50 with frequent bar visits also show strong acceptance
   - Age is a strong predictor of coupon acceptance

3. **Passenger Influence** ✓
   - Drivers traveling **alone, with friends, or with partners** are more likely to accept
   - Drivers with **children in the car significantly less likely** to accept
   - Social context heavily impacts decision

4. **Marital Status** ✓
   - Widowed drivers show lower acceptance rates
   - Non-widowed status correlates with higher acceptance

5. **Social Lifestyle** ✓
   - Frequent restaurant visitors (especially budget restaurants)
   - Higher income households show different patterns
   - Active social engagement predicts coupon acceptance

#### Hypothesis

**Target Profile for Bar Coupons:**
- Socially active drivers
- Younger age (under 50)
- Frequent bar/restaurant visitors
- Traveling without children
- Non-widowed status

These drivers view bar coupons as fitting their lifestyle and are more likely to make a detour.

---

### Coffee House Coupon Analysis

**Overall Acceptance Rate**: Coffee house coupons show distinct time-based patterns.

#### Key Patterns:

1. **Time is Critical** 
   - **7 AM**: Highest acceptance (morning commute)
   - **10 AM**: High acceptance (mid-morning)
   - **2 PM & 6 PM**: Low acceptance (peak driving times)
   - **Evening**: Some acceptance on trips back home

2. **Destination Matters** 
   - **7 AM + Work destination**: Peak acceptance (commuters)
   - **10 AM + No urgent destination**: High acceptance (leisure/flexible schedule)
   - **2 PM & 6 PM + Any destination**: Low acceptance
   - **Evening + Home destination**: Moderate acceptance

3. **Behavioral Insights**
   - Coffee house coupons work well during commute hours
   - Flexible schedule holders (no urgent destination) accept during off-peak times
   - Time pressure reduces coupon acceptance

#### Hypothesis

**Target Profile for Coffee House Coupons:**
- Morning commuters (7 AM to work)
- Mid-morning drivers with flexible schedules
- People on routine/habitual routes
- Less dependent on day/weather compared to other coupon types

---

## Methodology

- **Data Cleaning**: Removed records with missing critical information
- **Statistical Analysis**: Calculated acceptance rates across demographic segments
- **Visualization**: Used heatmaps and groupby analysis to identify patterns
- **Comparative Analysis**: Compared target groups vs. control groups

## Insights for Marketing

1. **Bar Coupons**: Target socially-active, younger demographic without children
2. **Coffee House Coupons**: Time-targeted campaigns (morning/commute focused)
3. **Coupon Timing**: Delivery time should match driver's schedule and destination
4. **Social Context**: Passenger type is crucial for restaurant/bar venues

## Files

- `coupons.csv` - Main dataset
- `prompt.ipynb` - Analysis notebook with code and visualizations
- `README.md` - This file

## Tools Used

- Python 3
- Pandas (data manipulation)
- Matplotlib & Seaborn (visualizations)
- NumPy (numerical analysis)

---

*Analysis completed as part of Machine Learning coursework - Module 5*
