# Financial-Analysis-of-Top-12-German-Companies-Using-Excel
The project aims to analyse financial performance of top 12 German Companies by demonstrating the use of tools in Excel.
|Project Overview
The project aims to analyse financial performance of top 12 German Companies by demonstrating the use of tools in Excel. The data for this analysis is sourced from Kaggle (link mentioned at the end) and it spans quarterly from 2017 to 2024. 

|Dataset Description 
The data set contained the columns of company, period, revenue, net income, liabilities, assets, liabilities, equity, ROA (return on assets), ROE (return on equity) and debt to equity.

|Data Exploration and Cleaning 
The data was without any duplicates or missing values. The format of the cells was checked, and few of them needed changes from general to number. Also, the ratios of ROA (Return on Assets), ROE (Return on Equity) and Debt to Equity were already calculated. However, they were recalculated to retain the formulas. Given the data, few more financial ratios were calculated i.e. Profit Margin and Asset Turnover. All this is done in the sheet titled “Ratio Calculation”.

|Data Transformation
The sheet “Cleaned Data” contains the data that has been cleaned and is used for analysis and visualisations. It was converted into Pivot Table to facilitate advanced analysis. Through XLOOKUP a new column of Sector is created by merging another table into the main data set, to show how companies are scattered over different sectors. This will enable sector-based analysis. The columns of Leverage and Efficiency are also added using the IF function of excel. To grasp a general outlook of the data, conditional formatting is done on all the ratios.

Formulas Used:
- Profit Margin = Profit/Revenue
-	Debt to Equity = Liabilities / Equity
-	Return on Assets = Net Income/ Assets
-	Return on Equity = Net Income/ Equity
-	Asset Turnover = Revenue/Assets

|Data Analysis
Data analysis is done in three dimensions. The first one is a Ratios analysis of all the 12 companies, which largely uses conditional formatting. The second one is Dashboard Analysis, which is using all the visualisations created from the data set.  The third one is Sector wise comparative analysis where slicers within the dashboard are used to breakdown the analysis into different sectors. Timeline is also inserted in the dashboard to facilitate the examination over different time periods. 

||Ratio Analysis
|||1.	ROA (Return on Assets)
The ROA shows how much profit is generated over the assets. In simple terms it shows how much profit is earned over $100 of assets (since it is a percentage therefore $100 is assumed as a           denomination). The higher this ratio is, the better it is. As it signifies that assets are operating efficiently to generate profit on them and their costs are covered. Top 10 highest values in the column of the ROA are highlighted as red. Apparently Volkswagen AG has the greatest number of highest ROA as compared to the rest of the German companies as concluded from the screenshot below: <img width="468" height="117" alt="image" src="https://github.com/user-attachments/assets/7e4b06a1-8e2c-4f6f-a917-3d203930154a" />

