# Product Funnel & Drop-Off Analysis
End-to-end analysis of user behavior across a product funnel to identify conversion gaps and drop-off insights using Python and Power BI.

# Project Overview

This project analyzes user behavior across a multi-stage product funnel to identify conversion bottlenecks, drop-off points, and optimization opportunities.

The analysis simulates real-world e-commerce user journeys, validates funnel integrity, computes stage-wise conversion and drop-off metrics, and presents insights using Power BI dashboards.

# Objectives

- Understand where and why users drop off in the funnel
- Measure conversion efficiency at each funnel stage
- Compare funnel performance by:
       Device type,
       Traffic source,
       Product category
- Deliver business-ready insights through interactive dashboards

# Funnel Stages

The funnel follows a standard e-commerce journey:
- Visit
- Product View
- Add to Cart
- Checkout
- Payment success

# Tools & Technologies

- Python (Data generation & analysis)
- Pandas, NumPy (Data manipulation)
- Power BI (Data modeling & visualization)
- DAX (Funnel metrics & calculations)

# Dataset Creation (Synthetic Data)

Since real production data was unavailable, a realistic synthetic dataset was generated to mimic actual user behavior.

**Dataset Characteristics**
- 10,000 unique users
- Sequential event tracking
- Time-based event progression
- User attributes:
     Device Type (Mobile, Desktop)
     Traffic Source (Organic, Ads, Referral, Social Media)
     Product Category (Electronics, Fashion, Home, Beauty, Sports)
     Transaction Price

**Funnel Probabilities**

| Stage Transition | Probability |
|------------------|-------------|
| Visit → Product View | 70% |
| Product View → Add to Cart | 55% |
| Add to Cart → Checkout | 60% |
| Checkout → Payment Success | 65% |

This mirrors realistic e-commerce drop-off behavior.

# Dashboards images
<img width="900" height="600" alt="Dashboard page 1" src="https://github.com/user-attachments/assets/dbe90bdf-15c6-4329-91ea-7e9992f5e6b9" />
<img width="900" height="600" alt="Dashboard page 2" src="https://github.com/user-attachments/assets/3661148f-ecdb-46a4-8a59-3d5402d1c213" />

# Power BI Dashboards Insights

**Funnel Overview**

- **Strong Top-of-Funnel Traffic**: The funnel begins with 10,000 unique users, providing a solid base for conversion analysis.

- **Modest Overall Conversion**: Only 14.81% of users complete a purchase, highlighting substantial drop-off potential typical of e-commerce funnels.

- **Confirmed Purchases**: 1,481 users completed payment, validating the conversion rate and funnel consistency.

- **Healthy Revenue**: Total revenue of 4M suggests high average order value or strong premium purchase contributions.

- **Balanced Revenue Channels**: Revenue is evenly distributed across traffic sources (Social Media, Ads, Organic, Referral), indicating diversified acquisition without over-reliance on a single channel.

- **Device Purchase Parity**: Desktop and Mobile purchases are nearly equal, showing no major device bias but reinforcing the importance of optimizing both experiences.

- **Mid-Funnel Friction**: User counts drop sharply between Product View → Add to Cart and Add to Cart → Checkout, revealing key optimization opportunities.

- **Stable Purchase Trends**: Daily purchases fluctuate but show no downward trend, useful for linking performance with campaigns or UX changes.


**Drop-Off Insights** -

- **High Funnel Loss**: Out of all users, 8,519 dropped off, resulting in an 85.19% drop-off rate, consistent with the 14.81% overall conversion rate, indicating significant optimization potential.

- **Stage-Wise User Decline**: User counts decrease at every funnel step, with the largest losses before checkout, especially between Product View and Add to Cart.

- **Device Impact**: Mobile users show higher drop-off than Desktop, particularly at Add to Cart and Checkout, suggesting mobile UX or performance issues.

- **Drop-Off Concentration**: The highest drop-off volumes occur at Add to Cart (~3.2K) and Product View (~3.0K), making these stages top priorities.

- **Traffic Source Behavior**: Drop-off rates are similar across traffic sources, indicating conversion friction is platform-wide rather than channel-specific.

- **Category Differences**: Fashion and Sports experience higher late-stage drop-offs, while Home performs better, pointing to category-specific purchase barriers.

# Business Recommendations

**Improve Product → Add to Cart Experience**
- Clear pricing & discounts
- Strong CTAs
- Social proof (reviews, ratings)

**Optimize Mobile Checkout**
- Reduce form fields
- Improve load performance
- Enable quick payment options

**Refine Traffic Acquisition**
- Improve ad targeting quality
- Align landing pages with user intent

**Category-Specific Improvements**
- Sports & Home: 
      - Better product descriptions
      - Clear return and delivery policies
