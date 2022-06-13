# MechaCar_Statistical_Analysis


## Linear Regression to Predict MPG

<ADD SCREENSHOT OF LINEAR REGRESSION>

Vehicle length and ground clearance proved a non-random amount of variance to the mpg values.

To show statistical significance, you need the p-value to be higher than 0.05. Our p-value was 5.35e-11, which is 
much smaller. Because of this value, the slope is not considered to be zero.

It's not the best predictor. The r-squared value is around 70% accurate, which isn't very high. Our p-value is also not very high showing that it
might not be statistically signifigant.


## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension 
coils must not exceed 100 pounds per square inch. 

<ADD TOTAL SUMMARY PIC>

Looking at the chart for the total summary for all three lots, we can see that the
variance is 62.29, which is below the 100 PSI that the coils can handle. But how do we 
know which Lot is contributing where? 

<ADD LOT SUMMARY PIC>

When we look at the statistics for each lot indiviually, we see that the variance for Lot1 is .98, the variance for Lot2 is 7.46, 
which are both below our limit of 100 PSI. When we look at Lot3, the variance is 170.28 
which exceeds our limit of 100 PSI.


## T-Tests on Suspension Coils

<ADD T-TEST PIC>

When performing the t-test for the overall metrics, our p-value is .060 which is above our
significance level of 0.05, so we can assume it is not significant. 

We then performed the same t-test but on each lot separately instead of together.

<ADD T-TEST LOT1>

On Lot1, we can see the p-value is 1 which is over the 0.05 significance level, rendering
this test insignificant.

<ADD T-TEST LOT2>

On Lot2, the p-value is 0.60 which is considerably higher than the 0.05 significance
level, so this too insignificant.

<ADD T-TEST LOT3>

On Lot3, the p-value is .04, which is just below our significance level of 0.05, so this
one is considered significant.


## Study Design: MechaCar vs Competition

Lately, with all that is going on overseas, the gas price here has skyrocketed. I think a study that 
compares city and highway fuel efficiencies, would be a great design. I think the main metric to be
used would be the mpg rating. The null hypothesis would be that the city and highway fuel efficiency is the
same across all vehicles. The alternative hypothesis is that the city and highway fuel efficiency is different
across different vehicles.

I would use a two sample t-test to compare different mpg ratings between cars. If there was a certain mpg rating you
were hoping a new vehicle would have, it would be easy to insert it into a t-test as we did with the PSI rating
in this challenge. You'd be able to see if there was a significance value over 0.05 to see how efficient the 
vehicle would be. Data needed to run this test would be the means and variance levels of each vehicle.
