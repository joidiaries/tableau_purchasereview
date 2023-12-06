# TABLEAU - EXCEL PROJECT : WEST COAST  - PURCHASE REVIEW

## This is a sample project to showcase Excel and Tableau skills.
### Link: [Tableau Public](https://public.tableau.com/app/profile/joi.diaries/viz/WestCoastPurchaseReview/Dashboard1#1).

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/3beb1d4f-7acc-460f-bcc3-3a069a03d054)


> **GOAL:** 
> 1. Use MS Excel skills to manipulate data in preparation for visualization
> 2. Use Tableau skills to effectively visualize data for meaningful data-driven decisions.


### Here are the **questions** we want to answer:
1. Which vendor gives the highest savings in USD?
2. Which buyer has the highest item receivable or "undelivered" in USD?
3. Which location has the highest spend (possible expansion)?

### Data:
It is about the purchasing transactions made between 2019-2022. Made this data based on my 5 years experience in Supply Chain. I made this data similar to extracts from systems like SAP, Coupa and Oracle.

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/380f8ab7-31be-4d6d-85e7-571b4be3f387)


### Data Cleaning and Processing:
1. Get year from Document Date.
   
![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/4f02779b-cc7d-4fb3-b986-0dc9a90e097d)


2. Connecting 2 tables using VLOOKUP function -- this is to group the items in column D, which will result to shorter dropdown, in case the viewer would want one.
   
![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/817475ba-e8cb-4306-b297-5c28d00d50ec)


3. Converting CAD currency to USD.

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/3885d2b4-99bf-4676-94ad-19229f779e44)

4. Simple computation [(Ordered Quantity - Delivered Quantity) * Amount in USD] to get the Paid Amount, assuming payment is cash on delivery basis.
   
![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/1dc3643d-bd95-4cb8-819b-d44ab9d6ff1f)

5. Extracting savings percentage from text using REGEXEXTRACT.

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/94228e9b-c6be-4559-8ae6-87271eb17dc2)

### Findings
1. Which vendor gives the highest savings in USD? --> Omnisource Supplies (answer may vary if filtered per year, store location and buyer)

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/f5dbcc0d-c1c9-4321-96fc-e92464059173)

2. Which buyer has the highest item receivable or "undelivered" in USD? --> Jessica Brown. Though she has the highest spend, she also has the highest undelivered items. She should follow-up with her suppliers the orders to avoid further delay.

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/9328a5c8-b922-41d9-8e2e-95f112a5a138)


3. Which location has the highest spend (possible expansion)? Arizona (answer may vary if filtered per year, vendor and buyer)

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/11bfa1ef-1c5b-4631-a2d1-9769436f9ed4)



### Recommendation
1. This is only a demo for Excel-Tableau but for projects to be maintained weekly or monthly, it is better to have Tableau connected to the source of data. This is for the analyst to have more time doing the analysis than repeating manual work of extracting data.
2. The spend data is decreasing -- which should not be normal if the company wants expansion. This has to be investigated.

![image](https://github.com/joidiaries/tableau_purchasereview/assets/150142726/40c9fb4a-06e2-445f-a539-62ca7fc13156)

