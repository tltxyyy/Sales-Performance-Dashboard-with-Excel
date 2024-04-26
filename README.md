# Sales-Performance-Dashboard-with-Excel

## Main Aim
* Create a robust and user-friendly dashboard that provides actionable insights at a glance. The dashboards serves a high level view of sales performance, by brand, vendor and category against the forecast for the entire purchasing team to be used during negotiations and reporting.
* All data cleaning and dasboards are done solely in Microsft Excel to ensure ease of accessibility for the rest of the team.
* Sales and Forecast datasets are fed into the dashboard mainly using sumifs formula.


## Dataset
Sample Sales Dataset (data is extracted separately by location):
![Sample Sales Dataset](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/dc7248bb-2ff6-4c62-ab57-558fbd3b8ff9)

Sample Raw Forecast data (data is extracted separately by location and year):
![Sample FC Data SYD](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/c78b8c47-b7ba-4aed-89be-d47ba78d7425)

Aggregated Forecast that combines raw forecast datasets from each location and year to one sheet:
![Sample Aggregated FC Data](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/5193b4c6-7f63-4f42-8496-624ec813549b)

## User Guide
The first sheet of this Excel workbook contains a user guide. With this the dashboard should be intuitive for even those who sees it for the first time.

<img width="422" alt="image" src="https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/7093585e-3124-4cee-8c9e-e172b3b0ea64">


## Dashboard Design
Two kinds of dashboards are created:
1. Sales Table: Focuses on showing both sales figures and sales mix to aid buyers not only during negotiations but also when reporting to the management.
2. Visualisations: Provides more flexibility to play with other fields like timeline, sub-categories, shop locations that are not shown in the Sales Table.

### Sales Table
For both sales table dashboards, users can easily select the format and time period they want to see and analyse with the help of data validation:
* Year
* Month
* Format
  * Month-to-Date: Shows data from the beginning of selected month up to the current date or last day of selected month, whichever earlier.
  * Year-to-Date: Shows data from the beginning of  selected year up to the current date or last day of selected year, whichever earlier.

#### Methodology
The cornerstone of this approach was leveraging the SUMIFS formula, which allowed for dynamic and targeted data aggregation based on specified criteria. To facilitate the use of SUMIFS, data was strategically organised from various sources into a coherent and standardized format. A combination of other Excel functions like OFFSET and a myriad of date functions to enhance the dashboard's functionality. As the objective is to make this dashboard reusable and easily accessible, the most effective and simplest ways are used to solve what might seem to be a complicated query.

#### 1. Main table showing aggregated sales

Sales mix by vendor and category are conditional formatted to make patterns and trends more apparent. Intuitive icons are also thoughtfully added like green ticks for when sales hit forecast and upwards arrow for when sales this year went above last year's.

![DB Main](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/645d78c9-2fee-46e3-abb9-b3a4f6032bf1)

*This table view is not the full view as some cells are currently grouped. See the next table below for full view.*


#### 2. Table that can be filtered by sales outlet
As aggregated sales in the entire region can only let us see in high level how the company is performing, there is a need to filter and display sales performance by each outlet as well.

***Filtered Outlet 1***

![DB syd](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/1f4fbe4a-5f9a-4d25-95db-086f92204569)

***Filtered Outlet 2***

Further conditional formatting serves to grey out those brands that are not in the outlet.

![DB GC](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/c2afabe9-e70c-4c75-a936-97b1d0348e2e)

### Visualisations
Although still in progress, the visualisations has served to be useful during negotiations when answering questions for suppliers and planning for brands in different locations. This dashboard was designed for more flexibility allowing the user to not just filter by outlet and brand but also select the range of timeline freely in denominations of months. By visualising the sales in line graph, users can also understand the trend easily

####
Pivot tables and pivot charts are utilised to create the visualisations here. Slicers are also leveraged upon to make the dashboard more interactive and dynamic.

#### 1. Visualisation Dashboard 1
![Dashboard Visualisations - High level](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/9302edcb-423e-46d5-88b4-c700b93a9d89)

#### 2. Visualisation Dashboard 1
![Dashboard Visualisations - Shop level](https://github.com/tltxyyy/Sales-Performance-Dashboard-with-Excel/assets/69724535/6e98da0b-abf6-41d0-876f-6886041fb2dd)
