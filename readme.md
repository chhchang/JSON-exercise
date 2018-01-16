# JSON-exercise
****
### The Data
+ Projects funded by the World Bank
+ Data source: http://jsonstudio.com/resources/

### The Exercise
1. Find the 10 countries with most projects
2. Find the top 10 major project themes (using column 'mjtheme_namecode')
3. In 2. above you will notice that some entries have only the code and the name is missing. Create a dataframe with the missing names filled in.
****
### The Approach
1. Use .groupby() to count the number of projects by each country.

2. Use normalization to create tables from nested element for major project theme.

3. Clean data by fill in missing data with NaNs and perform backward fill.

4. Use .groupby() again to find the top 10 major project themes.
