# Task 6: Frame Hypotheses

# Hypothesis Testing Plan

## Business Context

The company introduced a new onboarding and activation campaign to improve user activation and conversion. The objective of this experiment is to determine whether the new onboarding experience should be rolled out to all users.

The primary business decision depends on whether the Treatment group demonstrates a statistically significant improvement in the selected North Star Metric compared to the Control group.

---

## Metric Being Tested

**User Activation Rate (Onboarding Completion Rate)**

### Definition

```text
User Activation Rate = Users Who Completed Onboarding ÷ Total Users
```

### Reason for Choosing This Metric

User Activation Rate was selected as the North Star Metric because:

- It directly measures onboarding effectiveness.
- It reflects whether users successfully reach the product's initial value.
- Activated users are more likely to engage, convert, and retain over time.
- It aligns closely with the experiment's objective of improving early user engagement.

---

## Null Hypothesis (H₀)

The new onboarding campaign does not improve the User Activation Rate.

```text
H₀: Treatment Activation Rate ≤ Control Activation Rate
```

There is no meaningful improvement in onboarding completion among users exposed to the new experience.

---

## Alternative Hypothesis (H₁)

The new onboarding campaign improves the User Activation Rate.

```text
H₁: Treatment Activation Rate > Control Activation Rate
```

Users exposed to the Treatment experience complete onboarding at a higher rate than users in the Control group.

---

## Type of Test

**One-Tailed Test**

### Reason

The business objective is specifically to determine whether the new onboarding campaign performs better than the existing experience.

The experiment is not concerned with identifying any difference in either direction; it is focused on detecting a positive improvement.

Therefore, a one-tailed test is appropriate.

---

## Significance Level

```text
α = 0.05
```

### Interpretation

A 5% significance level means that the company is willing to accept a 5% probability of incorrectly concluding that the Treatment performs better when it actually does not.

---

## Decision Rule

### Reject the Null Hypothesis

If:

```text
p-value < 0.05
```


**Conclusion:**

- The Treatment group shows a statistically significant improvement in User Activation Rate.
- Evidence supports rolling out the new onboarding experience.

### Fail to Reject the Null Hypothesis

If:

```text
p-value ≥ 0.05
```

**Conclusion:**

- There is insufficient evidence that the Treatment improves User Activation Rate.
- Additional testing or investigation may be required before rollout.

---

## Interpretation Logic

The hypothesis test will compare the User Activation Rate between the Control and Treatment groups.

### Possible Outcomes

| Result | Interpretation |
|----------|----------|
| Higher activation rate and p-value < 0.05 | Strong evidence that the new onboarding experience is effective |
| Higher activation rate but p-value ≥ 0.05 | Improvement may be due to random variation |
| Lower activation rate | Existing onboarding experience should be retained |

The final business recommendation will consider both statistical significance and guardrail metrics such as refund rate, support ticket rate, and user satisfaction before deciding on a full rollout.

---

## Business Decision Link

This hypothesis directly supports the business decision of whether the new onboarding campaign should be launched to all users.

If the Treatment group significantly increases User Activation Rate without creating unacceptable negative effects on guardrail metrics, the company should proceed with a full rollout. Otherwise, the onboarding experience should be revised or tested further before deployment.

# Task 7: Perform Hypothesis or A/B Test Analysis

# Hypothesis Test Results

## Test Performed

Two-Proportion Z-Test

### Metric Tested

User Activation Rate (Onboarding Completion Rate)

The objective was to determine whether the new onboarding campaign increased the proportion of users completing onboarding compared to the existing experience.

---

## Test Inputs

| Metric | Control | Treatment |
|----------|----------:|----------:|
| Users | 690 | 710 |
| Activated Users | 108 | 150 |
| Activation Rate | 15.65% | 21.13% |

---

## Hypotheses

### Null Hypothesis (H₀)

The new onboarding campaign does not improve User Activation Rate.

```text
H₀: Treatment Activation Rate ≤ Control Activation Rate
```

### Alternative Hypothesis (H₁)

The new onboarding campaign improves User Activation Rate.

```text
H₁: Treatment Activation Rate > Control Activation Rate
```

---

## Significance Level

```text
α = 0.05
```

---

## Test Output

| Statistic | Value |
|------------|--------:|
| Pooled Proportion | 0.1843 |
| Standard Error | 0.0207 |
| Z Score | 2.65 |
| P Value | 0.0040 |

---

## Decision Rule

Reject the null hypothesis if:

```text
p-value < 0.05
```

Result:

```text
0.0040 < 0.05
```

Decision:

**Reject H₀**

---

## Business Interpretation

The Treatment group achieved a significantly higher User Activation Rate than the Control group.

- Control Activation Rate: 15.65%
- Treatment Activation Rate: 21.13%
- Improvement: +5.48 percentage points

The probability that this improvement occurred by random chance is very low (p-value = 0.004).

This provides strong statistical evidence that the new onboarding campaign improves user activation and supports consideration of a broader rollout.

However, guardrail metrics such as support ticket rate and refund rate should also be evaluated before making a final business recommendation.