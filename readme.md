# Business Problem Statement

The company has introduced a new onboarding and activation campaign for its subscription-based digital product. Users were randomly assigned to either:

- **Control Group** – Existing onboarding experience
- **Treatment Group** – New onboarding and activation campaign

## Business Decision

The primary business decision is whether the new onboarding experience should be rolled out to all users.

## Stakeholders Impacted

This decision impacts:

- Product Management Team
- Growth and Marketing Teams
- Customer Success Team
- Business Leadership
- Future Users of the Platform

## Success Metric

The primary objective of the experiment is to improve:

- User Conversion Rate
- User Activation Rate
- Early User Engagement

The treatment group should demonstrate measurable improvement over the control group.

## Risks to Monitor

While increasing conversion and engagement, the company must ensure the new experience does not negatively impact:

- User Retention
- Churn Rate
- Customer Satisfaction
- Support Ticket Volume
- Overall User Experience

These are considered **guardrail metrics** and must remain stable or improve.

## Evidence Required Before Recommendation

Before recommending a full rollout, the following evidence is required:

1. The treatment group performs better than the control group on primary success metrics.
2. The observed improvement is statistically significant.
3. Guardrail metrics do not show negative impact.
4. The expected business value justifies implementation costs.

## Expected Outcome

Based on the experiment results, a recommendation will be made to:

- Roll out the new onboarding experience to all users.
- Continue testing and collect more data.
- Retain the existing onboarding experience.

# North Star Metric

## Selected North Star Metric

**User Activation Rate**

User Activation Rate is the percentage of users who complete the key activation event during onboarding and reach the point where they experience the core value of the product.

## Why This Is the Main Success Metric

The objective of the experiment is to improve onboarding and early user engagement. Activation is the most important milestone because it measures whether users successfully reach the product's core value after signing up.

A higher activation rate indicates that the onboarding experience is effectively helping users understand and adopt the product. Users who become activated are more likely to engage regularly, convert into paying customers, and remain subscribed over time.

## Why Other Metrics Are Supporting Metrics

While other metrics provide valuable insights, they do not directly measure onboarding success:

- **Conversion Rate:** Measures whether users subscribe or purchase, but does not indicate whether they successfully experienced the product's value.
- **Engagement Metrics:** Show user activity levels but may not reflect successful onboarding.
- **Retention Rate:** Measures long-term success but occurs after activation.
- **Revenue Metrics:** Reflect business outcomes but are influenced by many factors beyond onboarding.

These metrics help validate results but are considered supporting metrics rather than the primary measure of onboarding effectiveness.

## Connection to Business Growth

User activation is strongly connected to business growth because activated users are more likely to:

- Continue using the product.
- Convert to paid subscriptions.
- Remain customers for longer periods.
- Generate higher lifetime value.

Improving activation creates a larger base of engaged users, which contributes directly to revenue growth and customer retention.

## Risks of Optimizing This Metric Blindly

Focusing only on activation rate can create unintended consequences:

- Users may be pushed through onboarding too aggressively, reducing satisfaction.
- The company may prioritize short-term activation at the expense of long-term retention.
- Users could complete activation actions without gaining genuine value from the product.
- Increased activation may lead to higher support requests or customer frustration.
- Artificial improvements in activation may not translate into revenue or retention gains.

For this reason, activation rate should be evaluated alongside guardrail metrics such as retention, churn, customer satisfaction, and support volume before making a rollout decision.

# KPI Tree

## North Star Metric

**User Activation Rate**

Percentage of new users who successfully complete the onboarding process and reach the product's key activation milestone.

### Primary Driver 1: Onboarding Completion

Measures how effectively users progress through the onboarding flow.

Sub-Drivers:
- Onboarding Completion Rate
- Time to Complete Onboarding

### Primary Driver 2: Feature Adoption

Measures whether users interact with the product's core features.

Sub-Drivers:
- First Key Action Completion Rate
- Number of Core Features Used

### Primary Driver 3: Early User Engagement

Measures user interaction shortly after onboarding.

Sub-Drivers:
- Day 1 Engagement Rate
- Average Sessions per User (First Week)

## Guardrail Metrics

These metrics ensure improvements in activation do not negatively affect user experience or business outcomes.

- User Retention Rate
- Customer Support Ticket Rate
- User Churn Rate
- Customer Satisfaction Score (CSAT)

## KPI Tree Layout

![KIP Tree Layout preview](screenshots/kpi_tree_preview.png)