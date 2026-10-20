# Method and limitations

## What the paper demonstrates

The investigation compares alternative mathematical shapes against grouped U.S. household-income data and asks whether an aggregate indicator alone can describe the circumstances of households across an income distribution. It examines the tradeoff between overall fit, local fit, and interpretability.

The original paper works through histogram-based descriptions, polynomial regression, exponential fitting of the upper-income tail, and a quadratic/exponential piecewise approximation. It also discusses a negative-binomial shape as a possible comparison, but does not complete or validate a negative-binomial simulation.

## Retrospective qualifications

1. **GDP and household income measure different things.** GDP is a measure of production, not a direct measure of household income or well-being. A divergence between the two does not by itself establish the cause of inequality.
2. **The observations are households, not individuals.** Household size and composition matter when interpreting the table.
3. **Appendix A is only partially reproduced in the paper.** Its complete price-basis and survey-method footnotes are not present. Cross-year real-income claims should therefore be checked against the original Census source before being treated as verified trends.
4. **Income-bracket widths are unequal.** The appendix percentages are probability masses for named brackets, not probability-density heights. A true density histogram would divide each mass by its bracket width.
5. **A continuous density must be normalized.** It should be non-negative and integrate to one over its domain. The original paper explicitly recognizes that normalization of the fitted piecewise model remained unresolved.
6. **Density and cumulative probability are different.** A density value at one point is not the probability of falling below that point; interval probabilities require integration.
7. **The piecewise cutoff was chosen from the observed 1967 shape.** It was not validated out of sample, and smoothness, parameter uncertainty, and stability across years were not established.
8. **Several socioeconomic interpretations in the original paper go beyond what the grouped data and regressions alone can prove.** This repository preserves the paper unchanged while presenting the quantitative modeling process more cautiously in the README.
9. **The original chi-square discussion is not reproduced as a validated model-accuracy result here.** The paper does not provide enough reproducible expected-count detail and fitted-parameter treatment to independently verify that goodness-of-fit calculation.

## Data transcription used in this repository

`data/selected-income-brackets.csv` transcribes the seven visible income bands used for 1967, 1990, and 2019 from Appendix A of the paper. Display labels abbreviate endpoints (for example, `$15-25k` represents `$15,000-$24,999`). The table excerpt does not provide the complete upper-income distribution, so no missing bands are imputed.

`assets/income-brackets.svg` is a new portfolio chart created from that transcription. It is not one of the original GeoGebra figures.
