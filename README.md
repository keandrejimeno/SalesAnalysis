
# Sales Analysis

This project consists of Power BI reports of the classic sample database "AdventureWorks" v. 2022, created as part of the suggested exercises in Microsoft's learning courses in preparation for the PL-300 certification exam.

## Overview

AdventureWorks is a global wholesaler company that sells and distributes bicycles and related products such as clothing for cycling, components and parts, and accessories to resellers. The database is generated and used by their sales department. It consists of 57,851 sales entries spanning Fiscal Year (FY) 2018 to FY 2020, with dimension tables of its corresponding salespersons, product IDs, and regions sold. It also includes target sales for FY 2021 designated for each salesperson.

The interactive report showcases the sales performances, profit analysis, and individual performances of salespersons.


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

![image](https://github.com/user-attachments/assets/2697cb3d-950c-4506-b22a-debf69c31bf1)


### Salesperson Performance

![image](https://github.com/user-attachments/assets/42e1e767-1351-440a-8f71-3867ff1a51fb)



## Insights 

- Sales have been consistently growing since FY2018, but Profit and Profit Margins fell behind and suffered a loss for the first time in the latest year, FY2020.
- Analyzing Profit Margins by Product Category, Bikes has had a small profit margin since its inception, and the turn to FY2020 broke and failed to recover.
- Salesperson Performances have been consistently well throughout FY2020.
- To stay afloat, the company must deal with the ironic problem of making their Bikes profitable to sell.

