# Hypothesis Test Notes

## Metric Being Tested

Paid Conversion Rate

This metric measures the percentage of users who converted from free/trial users into paid customers.

---

## Null Hypothesis (H0)

There is no significant difference in paid conversion rates between the Control group and the Treatment group.

H0: Control Conversion Rate = Treatment Conversion Rate

---

## Alternate Hypothesis (H1)

The Treatment group has a higher paid conversion rate than the Control group.

H1: Treatment Conversion Rate > Control Conversion Rate

---

## Type of Test

One-tailed test

This is because the business specifically wants to test whether the new onboarding flow improves conversions, not just whether it changes them.

---

## Significance Level

α = 0.05 (5%)

This means we accept a 5% chance of concluding there is an improvement when there is actually none.

---

## Reason for Choosing This Metric

Paid conversion rate is the most important metric because it directly measures business growth and revenue generation.

Improving onboarding should ideally increase the number of users becoming paying customers.

---

## Interpretation Logic

If p-value < 0.05:

* Reject the null hypothesis
* Conclude that the new onboarding flow significantly improves paid conversion

If p-value ≥ 0.05:

* Fail to reject the null hypothesis
* Conclude that there is not enough evidence that the new onboarding improves paid conversion

---

## Business Decision Connection

If the Treatment group shows a significantly higher conversion rate, the company can roll out the new onboarding flow to all users.

If there is no significant improvement, the company may keep the existing onboarding or test a new variation.


## Hypothesis Test Results

### Summary of Test Inputs

* Primary metric tested: Paid Conversion Rate
* Test type: A/B Test using Two-Sample t-Test (Unequal Variances)
* Control group: Existing onboarding flow
* Treatment group: New onboarding flow
* Significance level (α): 0.05
* Hypothesized mean difference: 0

---

### Test Output

* P-value: Less than 0.05

This indicates that the observed difference between the Control and Treatment groups is statistically significant.

---

### Decision Rule

* If p-value < 0.05 → Reject the Null Hypothesis
* If p-value ≥ 0.05 → Fail to Reject the Null Hypothesis

Result:
Since p-value < 0.05, the Null Hypothesis is rejected.

---

### Business Interpretation

The Treatment group shows a statistically significant improvement in paid conversion rate compared to the Control group.

This suggests that the new onboarding and activation campaign is more effective at converting users into paid customers.

Based on this result, the business can consider rolling out the Treatment onboarding flow to all users to improve revenue and customer acquisition.


## Guardrail Metrics Evaluation

To ensure the recommendation is not based only on conversion improvement, four guardrail metrics were evaluated.

### 1. Refund Rate

* Control: 0%
* Treatment: 0%

Interpretation:
There is no difference in refund rates between the two groups. This suggests that the increased conversions in the Treatment group are not causing additional dissatisfaction or low-quality purchases.

Risk Assessment:
No risk identified.

---

### 2. Support Ticket Rate

* Control: 14.72%
* Treatment: 24.76%

Interpretation:
The Treatment group has a noticeably higher support ticket rate compared to the Control group. This indicates that users may be facing more issues or confusion during the onboarding process.

Risk Assessment:
Moderate operational risk identified.

---

### 3. Average Days to Convert

* Control: 8.86 days
* Treatment: 6.40 days

Interpretation:
Users in the Treatment group convert faster than those in the Control group. This is a positive sign, showing improved efficiency in the onboarding process.

Risk Assessment:
No risk identified.

---

### 4. Average Engagement Score

* Control: 57.03
* Treatment: 62.93

Interpretation:
The Treatment group has a higher engagement score, indicating better interaction and involvement with the product after onboarding.

Risk Assessment:
No risk identified.

---

## Final Guardrail Conclusion

The Treatment group shows strong performance across most guardrail metrics:

* No increase in refunds
* Faster conversion time
* Higher engagement

However, the higher support ticket rate suggests there may be some onboarding friction that needs attention.

Overall, the Treatment flow appears beneficial and can be recommended for rollout, with additional monitoring of customer support impact.
