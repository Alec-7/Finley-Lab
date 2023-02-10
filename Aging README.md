Assay: The number of flies that die every day or several days (typically 3 times a week) is recorded until all flies are dead.

Output: A folder, with a .xlsx file for each experiment processed. Each file will have at least 5 sheets:

1. Average Lifespan Summary: The mean lifespan, along with standard deviation, SEM, and n values.
2. Pairwise Log-Rank Test: Significance values for a log-rank test, which shows if lifespan is significantly different between conditions
3. Percent Alive: Shows what percent of flies are alive at each day of age, which can be used to construct a Kaplan-Meier curve
4. Dates of Death: Each cell represents an individual fly, and stores the age of that fly when it died. This is used the calculate the data on the Average Lifespan Summary sheet
5. Average Lifespan t-test: Significance values for pairwise t-tests comparing average lifespan. The log-rank test is likely a better measure of significance than this test, and no tests of normality or variance are done before this test.

There may be 2 additional sheets:

1. Mortality Index: The age range used for the index, the number of flies alive and dead, and the results of a chi-square test. Multiple mortality indexes can be calculated at once.
2. Original Data: A copy of the data used for all calculations.

This program can be used for any survival assay. One notable example is a hard fast, where flies are kept on agar (which provides hydration but no nutrition) until death.

This program currently cannot account for escaped flies, or perform accurate calculations before all flies are dead.

Each column represents a condition, while each row represents an age. Each cell stores the number of flies in a condition that died at that age.

Metadata cannot be stored in the columns where data is recorded. It is recommended that metadata is stored in columns to the left of where data is stored. 
That way, you do not need to use the numCols variable to specify how many columns to process.

See comments in the code for instructions on altering variables for each analysis

