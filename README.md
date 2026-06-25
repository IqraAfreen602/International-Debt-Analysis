# International-Debt-Analysis-Using-SQL
1. Introduction: This project explores global debt data using PostgreSQL to analyze total debt, country-specific debt levels, and debt indicators.
2. Process and Query Logic
Step 1: Connecting to the Database

    Used the provided PostgreSQL connection string to access the database.

    Explored the dataset structure, identifying key tables and columns.

Step 2: Understanding the Dataset

    Identified key fields such as country_name, indicator_name, indicator_code, and debt

    Checked for missing values and inconsistencies in the data.

Step 3: Writing SQL Queries and Analysis

    Total Debt Calculation

        Used SUM(debt) to determine total global debt.

        Insight: The total recorded debt in the dataset is 3079735.08 (in millions).

    Counting Distinct Countries

        Used COUNT(DISTINCT country_name) to find the number of unique countries.

        Insight: The dataset contains 124 countries.

    Identifying Debt Indicators

        Queried DISTINCT indicator_name to list all debt measurement types.

        Insight: Found 27 different debt indicators.

    Highest Total Debt by Country

        Used ORDER BY debt DESC and LIMIT 1 to find the highest debt

        Insight: Country China has the highest debt of 96.2 billion.

    Average Debt by Indicator

        Used AVG(debt) grouped by indicator_name and indicator_code

        Insight: Indicator PPG, multilateral (DIS, current US$) has the highest average debt value.

  
    Most Common Debt Indicator

        Used COUNT(*) as frequency with GROUP BY indicator_name and ORDER BY frequency DESC LIMIT 1.

        Insight: Interest payments on external debt, long-term (INT, current US$) appears the most across countries.


3. Conclusion

This analysis provides insights into global debt distribution and key trends. Findings highlight economic disparities and areas for further analysis on debt sustainability.
