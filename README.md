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


<img width="295" height="157" alt="image" src="https://github.com/user-attachments/assets/fa879ed0-b57d-4ca7-be1f-e0881bdd0af2" />

||Dashboard Analysis

|||1.	Market Share (Pie Chart)
Sheet titled Pie Chart is depicting the market share of companies measured by average revenue. Since there are top 12 companies of Germany, they almost have a market share of 8% or 9%, signifying that all the companies are of equal strength in terms of market share. 

<img width="269" height="234" alt="image" src="https://github.com/user-attachments/assets/7d624e0d-aab9-4755-a70e-0425154f9c15" />


||2.	Composition of Balance Sheet (Stacked Bar Chart)
The stacked Bar Chart is depicting the composition of Balance Sheet of the 12 companies. Balance Sheet consists of Equity, Assets and Liabilities. Stack bar is giving a rough idea about how all the components of balance sheet are distributed. The stacked bar chart below shows that all the companies have highest composition of assets in their balance sheet as compared to  equity and liabilities.

<img width="466" height="127" alt="image" src="https://github.com/user-attachments/assets/52fd1e9e-10c6-4db2-8a88-4dabb7b27d98" />


|||3.	Revenue Trend (Line Graph)
Line Graph shows the trend of average revenue of all the companies over the years. The analysis through Line Chart is only meaningful if few companies are chosen at a single time. E.g. here only companies from automotive sector are chosen. 

<img width="452" height="141" alt="image" src="https://github.com/user-attachments/assets/1dc66906-7840-455c-827c-30eb88df0550" />

|||4.	Revenue to Income (Scatter Plot)
 To show the relationship between revenue and income, a Scatter Plot is drawn. A trend line is also included to look out for any outliers and to get. Apparently, there are no outliers and, revenue and income seem to have direct linear relationship as shown below. This also implies that none of the companies are going through a loss as there are no negative numbers in income side. 

 <img width="452" height="102" alt="image" src="https://github.com/user-attachments/assets/6ae8b586-3442-43f8-a1b3-cd4a54dd1b77" />

 |||5.	Asset Turnover (Bar Chart)
 The sheet titled “Asset Turnover” shows the average of asset turnover of all the 12 companies through a Bar Chart. From the figure it is evident that Allianz SE has the highest asset turnover, while, Deutsche Bank AG has the lowest asset turnover.

 <img width="452" height="222" alt="image" src="https://github.com/user-attachments/assets/e26e6cf5-4778-4174-9795-86510721e004" />

 |||6.	Comparison between ROA and ROE (Bar Chart)
 The Bar Chart is doing a comparative analysis between Return on Assets (ROA) and Return on Equity (ROE). In general, all the companies have lower ROA as compared to ROE. Allianz SE, Bayer AG, Daimler AG, Merck KGaA and Volkswagen AG are the top performers in ROE dimension. A trend of lower ROA as compared to ROE across the industry implies that shareholders are getting a reasonable return on their investments. However, the assets of the company are not generating as much return for the company as the equity. Lower ROA can be an efficiency issue, and the companies can get valuable insights by observing ROA as it could indicate outdated assets, and the company may need to upgrade its assets to increase ROA Debt to Equity.

 <img width="418" height="152" alt="image" src="https://github.com/user-attachments/assets/927bd206-c66b-4e1f-b443-e1ff8d926324" />

|||7.	Sectors/Tree Map
Tree map is displaying the breakdown of companies based on their sector. It is evident that Automobile has the largest chunk of companies as it occupies the largest area in tree map. Technology, telecommunications and engineering has the smallest number of companies. 

<img width="396" height="183" alt="image" src="https://github.com/user-attachments/assets/a1fdd768-22cf-4a38-bc34-c6a3ed72a729" />

||Analysis by sector

To grasp the overall trend and relationships within a sector, a slicer is inserted for sector only which is connected to all the visualisations within the dashboard. Each sector will be analysed by selecting that sector in the slicer. Sectors Engineering, Technology and Telecommunications cannot be analysed as there is one only company in each of these sectors and therefore, no comparative analysis can be done within the sector. 

|||1.	Automotive
By using inserted slicer of sector only automotive sector is chosen from the list of top 12 German Companies which has the largest share of companies in Germany’s top 12 companies. Figure 1 is summarising all the findings.  

<img width="451" height="152" alt="image" src="https://github.com/user-attachments/assets/baa36c07-2381-40cb-acf3-9a905491f52e" />

The pie chart shows the market share of each automotive company within its sector. Daimler AG is the biggest player in the sector with market share of 26%, while Porsche is the smallest player with 24% of market share. Volkswagen and BMW both have same market share of around 25% in the automobile sector. Line chart shows that all the four car companies had a sporadic trend in average revenue, however, BMW AG is able to achieve considerable hikes in its revenue (detected through numerous peaks in its trend).
The composition of balance sheet is very similar to all the rest of the top 12 German companies with assets being the largest component of the balance sheet. Volkswagen AG has highest asset turnover/efficiency, while Porsche is lowest. Bar chart shows that ROE is greater than ROA for all the companies, with Volkswagen AG and Daimler AG having highest ROE and Porsche AG being the lowest. From the overall analysis it can be concluded that Volkswagen AG is the strongest player in the automotive sector. 

|||2.	Chemicals
The Chemicals sector is the second largest sector in the top 12 companies of Germany. The Figure 2 shows the dashboard of the chemicals sector. BASF SE and Merck KGaA are the largest players with 34% share. While Bayer is the smallest share in the sector with 32% share. BASF SE is the most efficient company within the sector with highest asset turnover, with Merck KGaA ranking lowest in efficiency as shown in the dashboard. 

<img width="452" height="236" alt="image" src="https://github.com/user-attachments/assets/98578e4a-f10d-45c9-830c-a188a3e0b3f6" />

The composition of Balance Sheet is very similar, with all the companies having the largest chunk in assets. The revenue trend over the years is very similar, however when compared in terms of market share, Bayer is experiencing a steady decline in its revenue, signifying why it has smallest market share in the sector. Like the other top 12 companies, the chemical sector companies also have lower Return on Assets (ROA) than Return on Equity (ROE) with Merck KGaA and BASF SE having higher ROE than Bayer AG. Lastly, as expected, the revenue to income relationship is linear, as shown by the scatter plot and is very close the predicted trend. It can be concluded that Merck KGaA and BASF SE are in neck-to-neck competition, while BASF SE is trying to catch up with them


|||3.	Financial Services
Only two financial services companies ended up in the sector of top 12 German companies as shown by the dashboard in Figure 3. Allianz SE ha the largest market share in the sector with 51% of the share, while Deutsche Bank AG has 49% share. The stacked bar chart shows that overall Deutsche Bank AG has larger balance sheet components as compared to Allianz SE. Both the companies, however, have assets as their largest component in the balance sheet.  Since both the companies are very competitive, their revenue trend over the years is also showing a very similar movement as shown in the line graph “Revenue Trend”. Allianz SE, being the ruling player in the sector, is having a considerable higher asset turnover/efficiency than its competitor Deutsche Bank AG. Allianz SE is having higher ROA and ROE as compared to its opponent, marking its dominance in yet another dimension. Like the rest of the industry, both the companies have higher ROE than ROA. The relationship between revenue and income is linear and is exactly at the line of trend. 

<img width="452" height="218" alt="image" src="https://github.com/user-attachments/assets/cce0d11e-ee1e-426f-a34d-d9e4b5ba4d35" />

||Conclusions
The dataset was set to analyse how the top 12 German companies are performing over different financial dimensions. From the analysis it can be concluded that Volkswagen is a strong player not only in its own sector of automotive but also in the whole industry. As it is having highest ROE and profit margin. Allianz SE is another notable player in the industry as it has highest asset turnover and one of the highest ROE as well. As all the companies are major players in the German market therefore, they were having very similar trend of various financial dimensions e.g. all the companies have higher ROE than their ROA, they all share linear and direct relationship of revenue to income and follow the same trend line. The data has few limitations as well. Other measures of efficiency can be deployed subject to the availability of data. As the asset turnover of all the companies is low which indicates that deeper investigation can be done on efficiency. ROE is greater than ROA for all the companies, a detailed breakdown of balance sheet can potentially unveil the reason for this trend, which is beyond the scope of this assignment.

|||Data Source
https://www.kaggle.com/datasets/heidarmirhajisadati/top-12-german-companies-financial-data?resource=download 

















