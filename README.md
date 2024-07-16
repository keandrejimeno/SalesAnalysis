# Sales Analysis

This project consists of Power BI reports of the classic sample database "AdventureWorks" v. 2022, created as part of the suggested exercises in Microsoft's learning courses in preparation for the PL-300 certification exam. The interactive report showcases the sales overview, profit analysis, and individual performances of the salespersons.

## About

AdventureWorks is a global wholesaler company that sells and distributes bicycles and related products such as clothing for cycling, components and parts, and accessories to resellers. The database is generated and used by their sales department. It consists of 57,851 sales entries spanning Fiscal Year (FY) 2018 to FY 2020, with dimension tables of its corresponding salespersons, product IDs, and regions sold. It also includes target sales for FY 2021 designated for each salesperson.

## Goal

The goal is to create a sales analysis BI report for AdventureWorks given the data. The report should include visualizations of the company's sales, profit and quantity sold in a given time range. The data can be presented in large categories (Countries, Product Categories). It should also include KPIs that showcases positive or negative performances. Furthermore, the BI report must have a salesperson performance analysis that can be exclusively viewed by the salesperson when opened in Power BI through his/her UPN.

## Report

[Here is the Sales Analysis Report file created](https://github.com/keandrejimeno/SalesAnalysis/blob/main/Sales%20Analysis%20Demo.pbix).

And its [pdf form](https://github.com/keandrejimeno/SalesAnalysis/blob/main/Sales%20Analysis%20Demo.pbix).

A dashboard cannot be provided since Power BI service are exclusive to organization accounts.

## Data Model

The data model consists of **two (2) Fact tables** (*Sales, Targets*) and **seven (7) Dimension tables** (*Reseller, Product, Salesperson, Date, Region, SalespersonRegion, Salesperson (Performance)*). 

![Data Model](https://github.com/keandrejimeno/portfolio/assets/173131794/09d280b1-0c81-402b-9e04-46718feb6074)

- *Sales* - records for every product sold transacted by their resellers alongside AdventureWork's assigned salesperson and sales region.
- *Targets* - monthly target sales for every salesperson, to be used to compare to actual sales performance
- *Reseller* - information on reseller clients
- *Product* - product information, including standard costs
- *Salesperson (Performance)* - salespersons of Adventure Works, including managers
- *Date* - date table with assigned hierarchical labels (fiscal year, quarter, month)
- *SalespersonRegion* - table of salespersons' assigned regions
- *Salesperson* - same as *Salesperson (Performance)* but used for *Targets* to compare with *Sales*


## Reports

The reports include **three (3) pages**, ***Overview***, ***Profit***, and ***My Performance***

- ***Overview*** - An overview of KPIs, sales, profit margin and quantity sold tracked through visualizations with selectable fiscal years and regions to filter.
- ***Profit*** - In-depth details centered around profit, with an interactable matrix of the complete summary of sales records.
- ***My Performance*** - Indicators and visualizations showcasing an individual salesperson's performance with RLS implemented.

### Overview

![image](https://github.com/user-attachments/assets/86dadf19-45f2-4f48-9314-84fef420811d)

### Profit

![image](https://github.com/user-attachments/assets/3ff9b254-d70b-4d32-b959-a5fa2c33ee86)


### Salesperson Performance

![image](https://github.com/user-attachments/assets/42e1e767-1351-440a-8f71-3867ff1a51fb)


## Insights 

- Sales have been consistently growing since FY2018, and the company has expanded its market from beginning in the US then to Europe and Australia throughout the years. However, Profit and Profit Margins fell behind and suffered a loss for the first time in the latest year, FY2020.
![image](https://github.com/user-attachments/assets/b4c3ea57-4dc8-45a1-bd3d-717662959911)
![image](https://github.com/user-attachments/assets/04bdf31e-4237-4f21-8fe4-a7b82e8ba140)
![image](https://github.com/user-attachments/assets/86dadf19-45f2-4f48-9314-84fef420811d)

- Seasonal patterns in quantity sold are consistent throughout the company's lifetime and even grows in FY2020, but profit has dipped significantly and struggled to remain positive by the turn of FY2020.
![image](https://github.com/user-attachments/assets/3e49ff61-0e66-4d32-8295-d9e8657ef407)

- Analyzing Profit Margins by Product Category, Bikes has had a small profit margin since its inception, and the turn to FY2020 broke and failed to recover. Other products maintain positive profit margins; Accessories being the most profitable.
![image](https://github.com/user-attachments/assets/a5d4ef80-9c74-4374-81db-e64c1cdf1851)

- Highlighting only FY2019, Bikes are still profitable, but have always been the lowest turnout for profit compared to other categories.
![image](https://github.com/user-attachments/assets/1c32fbd4-e631-4288-9ff7-74df7b9cd243)

- Highlighting FY2020, the profit margins for Bikes fell below 0%, which resulted in Quarter 1 having a huge loss, Quarters 2 and 3 profiting under $100k, and by Quarter 4 have yet to breakeven.
![image](https://github.com/user-attachments/assets/d86a65e0-b782-417e-b925-91038a8d523b)

- Investigating individual performances of the salespersons throughout FY2020, some have not met targets yet and some have already surpassed them, but through the performance of Brian Welcker, Director of Sales (who would be technically assigned in all regions through his subordinates), sales would have met annual targets, suggesting no slowdown of demand and growth.
![image](https://github.com/user-attachments/assets/6c928eae-f6e1-4140-ae6b-7be0c408a97c)
![image](https://github.com/user-attachments/assets/3cb19bc7-b2b3-4d21-b7d7-fc1afe1b8ab3)
![image](https://github.com/user-attachments/assets/ac6a7f54-4d1e-4069-9361-40238138409d)
![image](https://github.com/user-attachments/assets/70cad8fd-1cef-4e8e-9809-2e4fd559ec5c)
![image](https://github.com/user-attachments/assets/fb335f98-ddae-4324-8122-48d0a62383c3)
![image](https://github.com/user-attachments/assets/3646990f-0cd5-4e08-aabe-86bde57e2706)

## Conclusion

The Power BI report for the Sales Analysis is able to provide relevant and insightful visualizations and presentations about the sales performance for AdventureWorks. In conclusion, to stay afloat, **the company must deal with the ironic problem of making their Bikes profitable to sell**, either through increasing prices of Bikes (with an expected slowdown of sales and quantity demanded) or cutting costs of Bikes. Additionally, it can continue to prioritize other products that have shown consistently large profit margins. It would not be wise to conclude a slowdown of the company's growth or market tipping since sales and quantity continue to grow despite the loss in profits.

