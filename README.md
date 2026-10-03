# Superstore Sales Dashboard (Power BI)

This is a Power BI project I built while learning data analytics. It is a four page dashboard on US sales data from 2013 to 2016. I wanted to answer simple questions a business would actually ask: which regions sell the most, which products make money, and how sales move through the year.

## What is in the dashboard

**1. Sales Existence in US States**
A map with a bubble for every state, coloured by region (Central, East, South, West). Bigger bubble means more sales. There are year, month and region filters on the sides, so you can see how the picture changes for a single year or a single region. California and New York stand out right away.

**2. Zone Wise Sales Details**
One chart for each region (Central, East, South, West). The bars show sales by category and the line shows profit for the same category. This page is where it becomes obvious that high sales do not always mean high profit.

**3. Performance Matrix (sales vs profit)**
Sales broken down by region, customer segment, product category and state. The page opens in sales view. Ctrl + click on the button at the top to switch the same visuals to profit view. I did this with bookmarks so one page does the work of two.

**4. Monthly Sales Insight**
A line chart of monthly sales for each region, with four smaller charts below it comparing sales and cost month by month for Central, South, West and East. A year selector at the top filters everything.


## What I found

These are the things I noticed while going through the numbers (total sales across all years is about 2.30M):

- The West region is on top with about 725K in sales, followed by East at 679K, Central at 501K and South at 392K. South sells roughly 54% of what the West does.
- Consumer customers bring in a little over half of all sales (about 51%). Corporate is about 31% and Home Office about 19%.
- The three categories are very close. Technology leads with about 836K (36%), then Furniture at 742K (32%) and Office Supplies at 719K (31%).
- California and New York are the two biggest states by a clear margin, then Texas and Washington.
- Sales are low in the first half of the year and climb in the second half. September, November and December are the strongest months in most regions. East peaks in November and West peaks in December.
- Furniture is the weak spot. In Central and East the profit line for Furniture sits almost at zero even though the sales bars are large. In the West, Furniture has the highest sales of any category but the lowest profit.
- On the monthly cost vs sales charts, cost follows sales closely in almost every month, which means the margins are thin.

## How I built it

1. Loaded the sales data into Power BI.
2. Cleaned it in Power Query Editor: fixed data types, checked for blanks and combined the regional data into a single table.
3. Rechecked the totals in Excel to make sure the numbers in Power BI matched.
4. Created the measures and the visuals, then added slicers for year, month and region.
5. Used bookmarks and buttons for the sales and profit toggle on the Performance Matrix page.
6. Designed the layout, colours and backgrounds myself so each page reads easily.

Tools: Power BI Desktop, Power Query, DAX, Excel.

## How to open it

1. Download the repository (green Code button, then Download ZIP) or clone it.
2. Install Power BI Desktop. It is free from the Microsoft website and works on Windows only.
3. Open `Sales-Dashboard.pbix` in Power BI Desktop.
4. Click through the four pages and try the slicers. Remember Ctrl + click on the Performance Matrix page for the profit view.

If the map shows up blank, check that map visuals are turned on in Power BI under File, Options, Security.

## Files

```
Sales-Dashboard.pbix     the Power BI report
images/                  screenshots of each page
README.md                this file
```

## What I would add next

- A profit margin percentage measure so Furniture can be compared more fairly with the other categories.
- A page on discounts and shipping, since they probably explain part of the low Furniture profit.
- Year over year growth cards at the top of each page.

## About me

I am Saurav Singh Rana, from Almora, Uttarakhand, currently in Noida learning data analytics (SQL, Excel and Power BI). I am looking for my first role as a data analyst.

Email: sr864238@gmail.com
LinkedIn: https://www.linkedin.com/in/saurav-rana2004?utm_source=share_via&utm_content=profile&utm_medium=member_android

Feedback and suggestions are welcome.
