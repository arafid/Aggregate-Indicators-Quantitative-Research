# Paper guide

This guide helps a reviewer navigate the original 16-page IB Mathematics: Applications & Interpretation HL investigation included in this repository.

## Pages 1-3 - Motivation and economic framing

The paper introduces the problem of relying on aggregate indicators such as GDP without looking at the distribution of household outcomes. It contrasts aggregate economic output with household-income measures and discusses inflation-adjusted purchasing power.

## Pages 4-5 - Probability-distribution framing

The paper introduces continuous probability distributions, then explains why the investigation uses grouped household-income frequencies and histograms instead of raw individual observations. The 1967 distribution is introduced here.

## Pages 6-9 - Regression and piecewise modeling

This is the mathematical core of the investigation. It explores:

- a high-degree polynomial fit,
- an exponential model,
- an exponential fit to the upper-income tail,
- a quadratic fit to the lower range, and
- a quadratic/exponential piecewise approximation around the observed 1967 shape.

The paper also discusses residual error, R-squared, interpretability, normalization, and the arbitrariness of a data-driven cutoff.

## Pages 10-12 - Alternative shapes and later-year comparisons

A negative-binomial form is discussed as a possible comparison but is not simulated or validated. The paper then compares the shapes of the 1990 and 2019 grouped income distributions with the 1967 distribution.

## Page 13 - Conclusion

The paper returns to its central argument: a single aggregate measure can hide meaningful distributional differences, so interpretation should consider additional indicators and the shape of the underlying data.

## Page 14 - Bibliography

The paper lists the sources used in the original investigation.

## Pages 15-16 - Appendix A

The appendix reproduces a U.S. Census Bureau household-income percentage-distribution table. The CSV in this repository transcribes only the seven visible brackets for 1967, 1990, and 2019 that are used in the portfolio chart.
