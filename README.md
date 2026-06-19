# LinkedIn Content Experimentation Framework

## Project Overview

This project analyzes the performance of two LinkedIn project showcase posts to understand how different content formats influence audience engagement, profile visibility, and overall content effectiveness.

The analysis compares:

1. **API Weather Dashboard** (Video Post)
2. **Healthcare Claims Fraud & Cost Analytics** (Carousel/Image Post)

Using LinkedIn analytics data, the project applies concepts from A/B testing, KPI analysis, experimental design, and business analytics to evaluate content performance and generate actionable insights.

---

## Business Problem

As an aspiring Data Analyst, sharing projects on LinkedIn is an important way to build visibility and attract recruiters.

The objective of this analysis was to determine:

- Which content format drives higher engagement?
- Which format encourages profile visits?
- Which content type generates more audience interaction?
- How can future LinkedIn posts be optimized using data-driven decisions?

---

## Dataset

### Source
LinkedIn Post Analytics

### Posts Analyzed

| Post | Format | Topic |
|--------|----------|----------|
| API Weather Dashboard | Video | Real-Time Weather Analytics |
| Healthcare Claims Fraud & Cost Analytics | Carousel/Image | Fraud Detection & Cost Analysis |

---

## Key Metrics (KPIs)

### Engagement Rate

Measures audience interaction relative to impressions.

```text
Engagement Rate = Total Engagements / Impressions × 100
```

### Profile View Rate

Measures how effectively a post drives profile visits.

```text
Profile View Rate = Profile Views / Impressions × 100
```

### Save Rate

Measures how often users save the content for future reference.

```text
Save Rate = Saves / Impressions × 100
```

### Click Through Rate (CTR)

Measures how often users click links from the post.

```text
CTR = Link Clicks / Impressions × 100
```

---

## Performance Comparison

| Metric | Weather Dashboard (Video) | Healthcare Analytics (Carousel) |
|----------|----------|----------|
| Impressions | 629 | 551 |
| Total Engagements | 12 | 7 |
| Engagement Rate | 1.91% | 1.27% |
| Profile Views | 2 | 5 |
| Profile View Rate | 0.32% | 0.91% |
| Saves | 2 | 0 |
| Save Rate | 0.32% | 0.00% |
| Link Clicks | 0 | 3 |
| CTR | 0.00% | 0.54% |

---

## Analysis & Findings

### 1. Video Content Generated Higher Engagement

The Weather Dashboard video post achieved:

- Higher impressions
- Higher engagement rate
- More content saves

This suggests that video content may be more effective at attracting user interaction and retaining viewer attention.

---

### 2. Carousel Content Generated Better Profile Conversion

The Healthcare Analytics post achieved:

- Higher profile views
- Higher click-through rate

This suggests that analytical project showcases may attract a more qualified audience interested in exploring the creator's profile and portfolio.

---

### 3. Different Formats Serve Different Objectives

| Objective | Better Performing Format |
|------------|--------------------------|
| Engagement | Video |
| Content Saves | Video |
| Profile Visits | Carousel |
| Link Clicks | Carousel |

This highlights the importance of aligning content format with business goals rather than optimizing solely for impressions.

---

## Business Recommendations

### If the Goal is Engagement

Use:

- Short-form project walkthrough videos
- Dashboard demonstrations
- Interactive visual content

### If the Goal is Recruiter Visibility

Use:

- Detailed project case studies
- Carousel posts
- Problem → Analysis → Insights storytelling

### Recommended Strategy

A hybrid content approach:

1. Publish a carousel explaining the business problem and insights.
2. Follow up with a short video demonstrating the solution.
3. Compare performance across both formats.

---

## Experimental Design Evaluation

### Is This a True A/B Test?

No.

Although two content formats were compared, multiple variables changed simultaneously:

- Content topic
- Post format
- Posting date
- Posting time
- Audience composition
- Content structure

Because multiple factors changed at once, causal conclusions cannot be drawn.

This project should be viewed as a **Content Performance Analysis** rather than a statistically valid A/B test.

---

## How a True A/B Test Would Be Conducted

### Control Group (A)

Healthcare Analytics Carousel

### Test Group (B)

Healthcare Analytics Video

Keep Constant:

- Posting day
- Posting time
- Hashtags
- Call-to-action (CTA)
- Content topic

Measure:

- Engagement Rate
- Profile View Rate
- Save Rate
- Click Through Rate
- Follower Growth

This would allow a more accurate evaluation of whether content format alone influences performance.

---

## SQL Analysis Example

```sql
SELECT
    post_name,
    impressions,
    engagements,
    ROUND(
        engagements * 100.0 / impressions,
        2
    ) AS engagement_rate,
    ROUND(
        profile_views * 100.0 / impressions,
        2
    ) AS profile_view_rate
FROM linkedin_post_metrics;
```

---

## Skills Demonstrated

- Data Analysis
- KPI Development
- Business Analytics
- Experimental Design
- A/B Testing Concepts
- SQL
- Power BI
- Data Visualization
- Stakeholder Reporting
- Insight Generation

---

## Key Takeaway

This project demonstrates how analytics can be applied beyond traditional business datasets. By leveraging LinkedIn content performance data, the analysis highlights the importance of defining success metrics, evaluating audience behavior, and designing controlled experiments to support data-driven decision-making.

The exercise also reinforced a critical analytical principle:

> Correlation does not imply causation.

A meaningful A/B test requires controlling external variables to isolate the true impact of a single change.
