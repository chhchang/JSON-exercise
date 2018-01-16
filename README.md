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
****
### The Result

|Country Name        | Projects|
| -------------------|:-------:|
| China              | 19      |
| Indonesia          | 19      |
| Vietnam            | 17      |
| India              | 16      |
| Yemen, Republic of | 13      |
| Nepal              | 12      |
| Bangladesh         | 12      |
| Morocco            | 12      |
| Mozambique         | 11      |
| Tanzania           | 10      |

|Theme Name                                   |Projects |
| --------------------------------------------|:-------:|
| Environment and natural resources management| 250     |
| Rural development                           | 216     |
| Human development                           | 210     |
| Public sector governance                    | 199     |
| Social protection and risk management       | 168     |
| Financial and private sector development    | 146     |
| Social dev/gender/inclusion                 | 130     |
| Trade and integration                       | 77      |
| Urban development                           | 50      |
| Economic management                         | 38      |
