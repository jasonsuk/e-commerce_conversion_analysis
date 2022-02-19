# A/B Test

This project is to perform a A/B test for a e-commerce website design change. The provided dataset already includes conversion records on **control** and **treatment** groups.

Supposedly, the old page design should be presented to the control goup and the new one only to the treatment group.

## Hypothesis set-up

The hypotheses, therefore, will be as following:

- $𝐻*0: 𝐶*{new} - C\_{old} <= 0 $
- $𝐻*1: 𝐶*{new} - C\_{old} > 0 $

where C*{new}, C*{old} standards for the mean conversion rate for the treatment and control group respectively.

Once the new page creates statistically significant increase in conversion compared to the old page, the null hypothesis ($𝐻_0$) can be rejected and the new page might be deployed (of course, practical consideration such as costs, resources must also be taken.)

## Methodology

The data cleaning will be performed to avoid no missing, duplicated or incorrect records.

To analyze the test results, three approaches will be taken:

- Simulation using probability : supposing that the null is correct, test how significant the observation is
- Z-test : using statsmodels package
- Regression : calculating p-value for the relationship between test groups and conversion rate
