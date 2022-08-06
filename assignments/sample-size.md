# Assignment: Calculate an experiment's sample-size requirement

[Sample size determination](https://en.wikipedia.org/wiki/Sample_size_determination) (AKA power analysis) is the process of calculating the number of participants an experiment will require to reach statistical significance.  This calculation requires the size of the effect to be known in advance, usually based on prior experiments.

For this assignment, imagine that you are proposing a project to test whether users will be more likely to comply with a warning if a popular 80s adjective is used to highlight which option is safe (e.g. not installing potentially risky software the user has just downloaded) and which option is risky (e.g. installing the software).  You see warnings like this when you download and run software on your computer.

You choose three positive adjectives to describe the safe option, resulting in four possibilities: “bodacious”, “righteous”, “tight”, and a control (no adjective).  You also choose two negative adjectives for the risky option, resulting in three possibilities: “gnarly”, “grody”, or a control (no adjective).  This yields a between-subjects 4x3 design: four treatments for different adjectives for the safe option crossed with 3 treatments for the risky option.  For example, a warning with the options "Run (grody)" and "Cancel (bodacious)" is in the `(grody, bodacious)` treatment group, and a warning with simply "Run" and "Cancel" is in the `(control, control)` treatment group.  This yields a total of 12 treatment groups to cover all possible combinations of positive and negative adjectives.

Using online participants and gratuities, you can run the study at a cost of $5 per participant.

<!-- TODO: Change these values slightly each semester -->
Assume that 50% of participants will typically choose the safe option, and a really great adjective could improve the proportion who choose the safe option to 60% (an impressive 10% increase over the 50 percentage point baseline).

How many participants and what budget would you need to have a 50% chance of seeing an effect that yields _p_\<=0.05 using a chi-square test, if you are indeed correct that there is an adjective that causes 60% of participants to take the safe option? (The simplest case is a single adjective having an impact and all of the others having no impact, as you don’t need to make any assumptions about the two individual contributions combined.)

The simplest way to determine this is through numerical analysis: build a 12x2 contingency table of hypothetical observed results where one adjective has a 60% compliance rate, i.e., 60% of participants choose the safe option, in all of the treatment groups in which that adjective appears.  All other adjectives have a 50% warning compliance rate.  Increase the absolute numbers of participants (keeping the ratios the same) until you reach the point where the chi-square test produces a p-value \<= 0.05.  We recommend you use the CHITEST function in Excel or Google Sheets to run the chi-square tests, unless you have familiarity with statistical software.

It might seem confusing that we went from a 4x3 design to a 12x2 table.  The 4x3 design gives us 12 groups of participants, but each participant in an experiment can have a range of outcomes.  In this experiment, some participants from each group choose the safe option and some choose the risky option.

Previous students have found [this video](https://www.youtube.com/watch?v=hpWdDmgsIRE) and [this video](https://www.youtube.com/watch?v=n06JNqE8kuE) helpful.  We strongly suggest watching both of these videos to understand how the chi-square calculation works.  Notice that the CHITEST function in Excel or Google Sheets requires expected values.  These values are [computed by a formula](http://www.stat.yale.edu/Courses/1997-98/101/chisq.htm) and should not be entered manually.  This is also explained in the videos.  The [documentation for CHITEST](https://support.microsoft.com/en-us/office/chitest-function-981ff871-b694-4134-848e-38ec704577ac) or the example in [Wikipedia](https://en.wikipedia.org/wiki/Chi-squared_test) in the section titled “Example chi-squared test for categorical data” provide the exact formula if you need a reference to it outside of the videos.

Once you have determined a minimum sample size to reach statistical significance, try playing with the data values.  Swap the values in one row or column with the values in another row or column.  How does this affect the p value?

Turn in the following items:
1. A document with screenshots, spreadsheets, or other evidence of the sample size needed to produce a p value just under 0.05.
2. Similar evidence for what happens to the p value when you move data around.  Swap rows and/or columns three times and document the the results after each swap.
