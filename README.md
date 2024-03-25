# Benchmark Bank Performance Analysis using Power BI

[Link to Dashboard](https://app.powerbi.com/reportEmbed?reportId=4aae5e8e-febd-48d3-a32f-629e5368d25e&autoAuth=true&ctid=c7e7e149-4fde-41b0-83ea-7a16989e67f8)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tools Used](#tools-used)
- [Data Analysis Process](#data-analysis-process)
   - [1. Data Collection from Web Scraping](#1-data-collection-from-web-scraping)
   - [2. Data Import in Power BI](#2-data-import-in-power-bi)
   - [3. Data Cleaning in Power BI](#3-data-cleaning-in-power-bi)
   - [4. Data Modeling in Power BI](#4-data-modeling-in-power-bi)
   - [5. Data Visualization in Power BI](#5-data-visualization-in-power-bi)
   - [6. Data Analysis in Power BI and Find Insights](#6-data-analysis-in-power-bi-and-find-insights)
   - [7. Deployment in Power BI to Get Final Report](#7-deployment-in-power-bi-to-get-final-report)
- [Dashboard Structure](#dashboard-structure)
- [Insights](#insights)
   - [1. Market Share Analysis](#1-market-share-analysis)
   - [2. Trend Analysis](#2-trend-analysis)
   - [3. Comparative Analysis](#3-comparative-analysis)
- [Conclusion](#conclusion)
- [Customization](#customization)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Overview

Welcome to the Comprehensive Analysis of Bank Performance through Credit and Debit Cards using Power BI! This dashboard is designed to provide a concise and visually appealing representation of key performance indicators (KPIs) using Credit Cards and Debit Cards in Power BI.

## Features

- **Interactive Cards:** Easily view and analyze important metrics at a glance.
- **Filtering:** Use slicers and filters to drill down into specific data subsets.
- **Date Range Selection:** Analyze trends over custom date ranges.
- **Responsive Design:** The dashboard is optimized for various screen sizes.

## Tools Used

- Python
- Power BI Desktop

## Data Analysis Process

### 1. Data Collection from Web Scraping

- The data for this dashboard was collected through web scraping from [Reserve Bank of India (RBI) website](https://www.rbi.org.in/Scripts/ATMView.aspx) for 5 years (2019 to 2023).
- Web Scraping using the "BeautifulSoup" Package in Python.
- The scraped data was exported as 60 Excel files (representing 60 months) and stored in one folder.

### 2. Data Import in Power BI

- Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
- Clone or download the repository and open the `.pbix` file in Power BI Desktop.
- Import the Excel files as year wise folder (Get Source - from Folder).
- For Combining files, Each table requires some basic cleaning like Renaming Column names for smooth merging.
- Finally, merging the files using M language "Table.Combine()" to consolidate data.

### 3. Data Cleaning in Power BI

- After all 60 files merged, Perform data cleaning tasks in Power BI, including:
  - Removing null values and errors to ensure data accuracy.
  - Removing unneccessary rows and columns.
  - Fill missing values
  - Promote Headers and Renaming Column names.

### 4. Data Modeling in Power BI

- Build a robust data model in Power BI by defining relationships between tables and creating calculated columns and measures.

### 5. Data Visualization in Power BI

- Utilize Power BI's visualization capabilities to create an intuitive and informative dashboard.
- Include interactive cards, charts, and other visuals to convey key insights.

### 6. Data Analysis in Power BI and Find Insights

- Leverage Power BI's analytical tools to perform in-depth data analysis.
- Use features such as filters, slicers, and date range selection to uncover trends and patterns.

### 7. Deployment in Power BI to Get Final Report

- Deploy the finalized dashboard in Power BI service for wider access.
- Ensure that the deployed version reflects the latest insights and updates.
- [Report link](https://app.powerbi.com/reportEmbed?reportId=4aae5e8e-febd-48d3-a32f-629e5368d25e&autoAuth=true&ctid=c7e7e149-4fde-41b0-83ea-7a16989e67f8)

## Dashboard Structure

- **Page 1: Overview**
    ![image](https://github.com/Afzal-14/gsgd/assets/120948536/fccd6e2a-6415-4c79-badd-5b1ce5037b65)


- **Page 2: Detailed Analysis**
    ![image](https://github.com/Afzal-14/gsgd/assets/120948536/0d666179-cd43-4eb6-ab76-94a7bd93e197)
    ![image](https://github.com/Afzal-14/gsgd/assets/120948536/b9e60df3-60ef-493b-97dc-2c3a937f676c)
    ![image](https://github.com/Afzal-14/gsgd/assets/120948536/8e7d06ca-2a6c-4180-95ca-b0b168431323)

## Insights

Here are some key insights derived from the visualizations in the dashboard:

### 1. Market Share Analysis:
   
   **Bank Market Share based on overall Cards**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/598748d5-d54c-4889-bf18-2a96a91d0412)
  
   Cards:
   - At 43.82%, STATE BANK OF INDIA had the highest market share in Cards, which was Infinity higher than JIO PAYMENTS BANK at 0.00%.
   - Across all 74 Bank Names, market share in Cards ranged from 0.00% to 43.82%.
      
   Transactions:
   - At 43.68%, STATE BANK OF INDIA had the highest market share in Transactions, which was Infinity higher than JIO PAYMENTS BANK at         0.00%.
   - Across all 74 Bank Names, market share in Transactions ranged from 0.00% to 43.68%.
   
   Spend:
   - At 42.27%, STATE BANK OF INDIA had the highest market share in Spend, which was Infinity higher than JIO PAYMENTS BANK at 0.00%.
   - Across all 74 Bank Names, market share in Spend ranged from 0.00% to 42.27%.

   **Bank Market Share based on Credit Cards**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/53b99a11-b0a0-480f-a5e1-8a7d7b70337a)
  
   Cards:
   - **Highest Market Share:** HDFC BANK LTD at 29.91%
   - **Followed by:** STATE BANK OF INDIA, ICICI BANK LTD
   - **Overall Range:** 0.00% to 29.91%
      
   Transactions:
   - **Highest Market Share:** HDFC BANK LTD at 35.51%
   - **Followed by:** STATE BANK OF INDIA, ICICI BANK LTD
   - **Overall Range:** 0.00% to 35.51%
   
   Spend:
   - **Highest Market Share:** HDFC BANK LTD at 38.69%
   - **Followed by:** STATE BANK OF INDIA, ICICI BANK LTD
   - **Overall Range:** 0.00% to 38.69%

   **Bank Market Share based on Debit Cards**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/495736e6-ed1a-4ab0-903c-bb5297839d74)

   Cards:
   - **Highest Market Share:** STATE BANK OF INDIA at 45.65%
   - **Followed by:** BANK OF BARODA, PAYTM PAYMENTS BANK
   - **Overall Range:** 0.00% to 45.65%
      
   Transactions:
   - **Highest Market Share:** STATE BANK OF INDIA at 51.15%
   - **Followed by:** HDFC BANK LTD, ICICI BANK LTD
   - **Overall Range:** 0.00% to 51.15%
   
   Spend:
   - **Highest Market Share:** STATE BANK OF INDIA at 51.88%
   - **Followed by:** HDFC BANK LTD, ICICI BANK LTD
   - **Overall Range:** 0.00% to 51.88%
     
### 2. Trend Analysis:

   **Overall Cards Trend over Time Period**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/20b48701-9461-4ab3-b222-bb23c1829ddc)

   Sum of Cards:
   - **Overall Trend:** Upward
   - **Increase Percentage:** 9.32%
   - **Period:** Tuesday, January 1, 2019, to Friday, December 1, 2023
   - **Details:**
     - Started trending up on Wednesday, September 1, 2021.
     - Increase by 7.56% (743,897,84) in 2.25 years.
     - Steepest decline from 968,566,586 to 952,901,809 between Tuesday, January 1, 2019, and Friday, March 1, 2019.
   
   Sum of Transactions:
   - **Overall Trend:** Downward
   - **Decrease Percentage:** 64.77%
   - **Period:** January 2019 to December 2023
   - **Details:**
     - Started trending down on April 2022.
     - Decrease by 10.07% (55,800,702) in 20 months.
     - Steepest decline from 1,312,677,563 to 918,059,593 between January 2020 and July 2020.
   
   Sum of Spend:
   - **Overall Trend:** Downward
   - **Decrease Percentage:** 42.73%
   - **Period:** January 2019 to December 2023
   - **Details:**
     - Started trending up on August 2020.
     - Increase by 20.02% (682,555,800,000) in 17 months.
     - Steepest decline from 4,246,109,000,000 to 3,274,022,200,000 between January 2020 and July 2020.

   **Credit Cards Trend over Time Period**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/8f9f9f34-d364-4b85-891c-91547df652d9)

   Sum of Cards:
   - **Overall Trend:** Upward
   - **Increase Percentage:** 116.74%
   - **Period:** Tuesday, January 1, 2019, to Friday, December 1, 2023
   - **Details:**
     - Started trending up on Wednesday, December 1, 2021.
     - Increase by 42.00% (28,955,912) in 2 years.
     - Steepest incline from 68,948,699 to 97,904,611 between Wednesday, December 1, 2021, and Friday, December 1, 2023.
   
   Sum of Transactions:
   - **Overall Trend:** Upward
   - **Increase Percentage:** 100.40%
   - **Period:** January 2019 to December 2023
   - **Details:**
     - Started trending up on March 2023.
     - Increase by 22.04% (58,070,552) in 9 months.
     - Steepest decline from 203,783,554 to 132,651,314 between January 2020 and July 2020.
   
   Sum of Spend:
   - **Overall Trend:** Upward
   - **Increase Percentage:** 198.34%
   - **Period:** January 2019 to December 2023
   - **Details:**
     - Started trending up on October 2020.
     - Increase by 154.45% (1,002,272,753,000) in 38 months.
     - Steepest incline from 648,919,600,000 to 1,651,192,353,000 between October 2020 and December 2023.

   **Debit Cards Trend over Time Period**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/3e9bfc13-77ee-4e61-b0c7-52848aeb178b)
 
   Sum of Cards:
   - **Overall Trend:** Upward
   - **Increase Percentage:** 4.06%
   - **Period:** Tuesday, January 1, 2019, to Friday, December 1, 2023
   - **Details:**
     - Started trending up on Tuesday, December 1, 2020.
     - Increase by 8.49% (75,234,376) in 3 years.
     - Steepest decline from 923,395,544 to 905,813,162 between Tuesday, January 1, 2019, and Friday, March 1, 2019.
   
   Sum of Transactions:
   - **Overall Trend:** Downward
   - **Decrease Percentage:** 85.90%
   - **Period:** January 2019 to December 2023
   - **Details:**
     - Started trending down on April 2022.
     - Decrease by 46.61% (154,370,071) in 20 months.
     - Steepest decline from 871,473,533 to 327,518,914 between January 2022 and March 2022.
   
   Sum of Spend:
   - **Overall Trend:** Downward
   - **Decrease Percentage:** 84.86%
   - **Period:** January 2019 to December 2023
   - **Details:**
     - Started trending down on April 2022.
     - Decrease by 26.32% (171,231,187,000) in 20 months.
     - Steepest decline from 3,456,251,600,000 to 640,518,647,000 between December 2021 and March 2022.

### 3. Comparative Analysis:

   **HDFC vs SBI  overall cards over Time Period**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/75959477-7bd6-4ca4-9179-b7db22197570)
   
   Volume of Cards:
   - **Trend Analysis:**
     - HDFC BANK LTD: 89.47% increase
     - STATE BANK OF INDIA: 21.88% decrease
     - Period: January 2019 to December 2023
   
   - **Details for STATE BANK OF INDIA in Volume of Cards:**
     - Started trending down on May 2023.
     - Decrease by 15.77% (45,865,736) in 7 months.
   
   Total Transactions:
   - **Trend Analysis:**
     - STATE BANK OF INDIA: 82.35% decrease
     - HDFC BANK LTD: 14.60% decrease
     - Period: January 2019 to December 2023
   
   - **Details for STATE BANK OF INDIA in Total Transactions:**
     - Started trending down on April 2022.
     - Decrease by 24.79% (33,838,260) in 20 months.
   
   Total Amount:  
   - **Trend Analysis:**
     - HDFC BANK LTD: 30.71% increase
     - STATE BANK OF INDIA: 68.12% decrease
     - Period: January 2019 to December 2023
   
   - **Details:**
     - Most recent anomaly: April 2020, HDFC BANK LTD with a low of 171,012,200,000.
     - Total Amount Comparison for HDFC BANK LTD started trending up on April 2023.
     - Increase by 12.45% (59,011,709,000) in 8 months.

   **HDFC vs SBI  Credit cards over Time Period**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/1645ebdb-3107-4f0a-8bae-3ba95aedd80a)
   
   Volume of Cards: 
   - **Trend Analysis:**
     - STATE BANK OF INDIA: 138.63% increase
     - HDFC BANK LTD: 60.82% increase
     - Period: January 2019 to December 2023
   
   - **Details for HDFC BANK LTD in Volume of Cards:**
     - Started trending up on March 2023.
     - Increase by 13.36% (2,342,158) in 9 months.
   
   Total Transactions: 
   - **Trend Analysis:**
     - HDFC BANK LTD: 93.07% increase
     - STATE BANK OF INDIA: 108.04% increase
     - Period: January 2019 to December 2023
   
   - **Details for HDFC BANK LTD in Total Transactions:**
     - Started trending up on May 2023.
     - Increase by 23.80% (16,040,143) in 7 months.
   
   Total Amount:
   - **Trend Analysis:**
     - HDFC BANK LTD: 189.99% increase
     - STATE BANK OF INDIA: 188.46% increase
     - Period: January 2019 to December 2023
   
   - **Details for STATE BANK OF INDIA in Total Amount:**
     - Started trending up on June 2023.
     - Increase by 17.09% (42,687,495,000) in 6 months.

   **HDFC vs SBI  Debit cards over Time Period**
     ![image](https://github.com/Afzal-14/gsgd/assets/120948536/e5d45cf5-9f0b-4685-beed-9fe8aa2a749e)
   
   Volume of Cards:
   - **Trend Analysis:**
     - HDFC BANK LTD: 102.95% increase
     - STATE BANK OF INDIA: 25.95% decrease
     - Period: January 2019 to December 2023
   
   - **Details for STATE BANK OF INDIA in Volume of Cards:**
     - Started trending down on June 2023.
     - Decrease by 15.90% (42,801,250) in 6 months.
   
   Total Transactions:
   - **Trend Analysis:**
     - STATE BANK OF INDIA: 91.17% decrease
     - HDFC BANK LTD: 70.39% decrease
     - Period: January 2019 to December 2023
   
   - **Details for HDFC BANK LTD in Total Transactions:**
     - Most interesting recent trend.
     - Started trending down on April 2022.
     - Decrease by 43.42% (18,949,399) in 20 months.
   
   Total Amount:
   - **Trend Analysis:**
     - STATE BANK OF INDIA: 90.23% decrease
     - HDFC BANK LTD: 66.35% decrease
     - Period: January 2019 to December 2023
   
   - **Details for HDFC BANK LTD in Total Amount:**
     - Started trending down on May 2022.
     - Decrease by 19.67% (20,877,485,000) in 19 months.
 
## Conclusion

  **Market Share:**
  - ***STATE BANK OF INDIA Dominance:***
    - STATE BANK OF INDIA emerges as a dominant player in both overall Cards and Debit Cards, boasting the highest market share.
    
  **Trend Analysis:**
  - ***Upward Trajectory in Overall Cards:***
    - Overall Cards exhibit a positive upward trend, indicating an increase in the usage or issuance of cards.
  - ***Robust Growth in Credit Cards:***
    - Credit Cards experience substantial growth, suggesting increased adoption and usage in the market.
  - ***Mixed Trends in Debit Cards:***
    - Debit Cards display a combination of upward and downward trends, showcasing fluctuations in usage and popularity.
  
  **Comparative Analysis:**
  - ***Consistent Positive Performance by HDFC BANK LTD:***
    - HDFC BANK LTD consistently demonstrates positive growth in both overall and credit cards, positioning itself as a strong and reliable performer.
  - ***Challenges Faced by STATE BANK OF INDIA:***
    - STATE BANK OF INDIA encounters challenges, particularly in Debit Cards, where a notable decline is observed, necessitating strategic considerations and interventions.

    These summarized insights provide a quick overview of the market dynamics, trends, and comparative performance between HDFC BANK LTD and STATE BANK OF INDIA. Refer to the detailed analysis for a more in-depth understanding.

    [Link to Dashboard](https://app.powerbi.com/reportEmbed?reportId=4aae5e8e-febd-48d3-a32f-629e5368d25e&autoAuth=true&ctid=c7e7e149-4fde-41b0-83ea-7a16989e67f8)
    
## Customization

Feel free to customize the dashboard to suit your specific needs. You can modify visuals, add additional cards, or integrate with other Power BI features.

## Contributing

We welcome contributions! If you have suggestions, improvements, or bug fixes, please create a pull request.

## Acknowledgments

Special thanks to Technocolabs and my team members for their contributions to this project.
