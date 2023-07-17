# Sql-Data-Analysis
Analyzing Covid data using Postgresql.
Report Title: Analysis of COVID-19 Data

1. Introduction:
   This report provides an analysis of COVID-19 data using the "covid_affected" and "covid_vaccination" tables. The objective is to gain insights into the global impact of the pandemic, assess the spread and severity of the virus in different countries, and evaluate the progress of vaccination efforts.

2. Data Filtering and Summarization:
   - Filtered the data to include records with a specified continent using the "WHERE" clause.
   - Calculated the total number of reported cases and deaths globally.

3. Percentage of Population Affected:
   - Investigated the percentage of population affected by COVID-19 in each country.
   - Utilized float casting to accurately compute the percentage of population affected.

4. Countries with High Death Rate:
   - Identified countries with the highest death rates based on the ratio of total deaths to total cases.
   - Grouped the data by country and sorted in descending order of the death rate.

5. Running Total of Cases in India:
   - Tracked the cumulative number of new cases in India over time using the "SUM" function and window function.

6. Highest Total Cases in a Month in India:
   - Determined the month with the highest total cases in India.
   - Grouped the data by month, sorted in descending order of total cases.

7. Percentage of Population Vaccinated:
   - Analyzed the percentage of population vaccinated in each country by joining the "covid_affected" and "covid_vaccination" tables.
   - Calculated the percentage of population vaccinated by dividing the number of vaccinated individuals by the country's population.

8. COVID-19 Cases Growth Rate in India:
   - Analyzed the growth rate of COVID-19 cases in India over the last 10 days.
   - Computed the growth rate as a percentage by comparing the current total cases with the cases reported 10 days prior.

9. Rate of Spread in India:
   - Grouped the rate of spread in India based on the number of new cases.
   - Categorized the rate of spread as "Fleeting," "Rapid," "Very High," "High," or "Low" based on predefined thresholds.

10. Average Number of Cases in Top 5 Spreading Countries:
    - Calculated the average number of COVID-19 cases in the top 5 countries with the highest total cases.
    - Joined the "covid_affected" and "covid_vaccination" tables, grouped the data by country, and computed the average.

11. Percentile Analysis of Total Cases:
    - Determined the percentile under which the total cases fall for each country and date combination.
    - Partitioned the data by country and sorted it by total cases, then assigned percentiles using the "NTILE" function.

12. Median of New COVID-19 Cases:
    - Computed the median of new COVID-19 cases in India.
    - Used the "percentile_disc" function to calculate the median value.

13. Conclusion:
    The analysis of COVID-19 data provided valuable insights into the global impact of the pandemic, the severity of the virus in different countries, and the progress of vaccination efforts. These findings can contribute to informed decision-making and effective strategies in combating the ongoing pandemic.

Note: The actions and findings mentioned in this report are based on the analysis of COVID-19 data and can be customized or expanded based on specific requirements or data availability.
