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
The ROA shows how much profit is generated over the assets. In simple terms it shows how much profit is earned over $100 of assets (since it is a percentage therefore $100 is assumed as a           denomination). The higher this ratio is, the better it is. As it signifies that assets are operating efficiently to generate profit on them and their costs are covered. Top 10 highest values in the column of the ROA are highlighted as red. Apparently Volkswagen AG has the greatest number of highest ROA as compared to the rest of the German companies as concluded from the screenshot below: 


  <img width="275" height="157" alt="image" src="https://github.com/user-attachments/assets/c9c08cca-9cdb-4c8a-a456-4b019896fe36" />

  |||2.	ROE (Return on Equity)
 The Return on Equity (ROE) shows how much the profit is generated on the total equity of the company. This ratio is quite significant as it shows the return of investment to the owners/shareholders of the company. The higher this ratio is, the better it is as it signifies to the owners/shareholders that their investment is not going in a loss. In the column of ROE, top 10 figures of ROE are highlighted green. From the screenshot below it shows that Siemens AG, Allianz SE and Deutsche Bank AG have the greatest number of highest ROE figures as shown in the next image:

 <img width="275" height="141" alt="image" src="https://github.com/user-attachments/assets/cbccc6e5-f664-403a-9dc8-19fd88819451" />

 |||3.	Debt to Equity and Leverage
 Leverage as calculated by Debt-to-Equity ratio depicts the composition of assets and liabilities of a company. There must be a fine balance between equity and debt of a company. Large companies usually have higher proportion of debt as compared to equity in their source of funding. It not only amplifies return on equity but also provides with ample source of funding as compared to equity market. How much leverage is ideal? Well, the answer varies from company to company. I have made a Leverage Column by applying IF function on Debt-to-Equity Column. All values in Debt to Equity greater than or equal to one are highlighted as Yellow and labelled as “High”, while all values less than one are highlighted as Green and labelled “Low”.  The leverage column shows that there is a good mix of high and low leverage companies. 

 |||4.	Asset Turnover/Efficiency
 Asset Turnover represents how quickly assets were turned over/refreshed to generate revenue.  It shows how much sales are generated for each dollar of assets. The higher the ratio is, the better it is. Theoretically, a ratio above 1 is ideal but not mandatory. The Asset Turnover Column in the Cleaned Data Sheet has red arrow showing all the figures less than 1. 

To further facilitate the analysis Efficiency column is created by using IF function on the Asset Turnover Column. Cells in Efficiency column are highlighted as red and labelled as “Low” if Asset Turnover value is equal or less than 1. Otherwise, the values greater than 1 will be labelled as “High” with yellow highlight. All the cells in the Efficiency Column turned out to be red signifying that all the companies have low level of efficiency. Due to limitations of data, further analysis cannot be done to verify it. 

|||5.	Profit Margin
Profit Margin represents profit as a percentage of revenue.  A higher percentage is desired. This ratio measure whether the company is capable enough to pay off its operating expenses from its revenue and generate a profit on top of it. Highest top 10 figures are highlighted as yellow in the Profit Margin column. The screenshot below shows that Volkswagen again, like ROA, has scored highest instances of high Profit Margin quarterly over the span of 8 years (2017 to 2024). 











