# Exercise 1 - Exercise 1 Description

In this exercise, we will create...

As a business analyst for the BestRun company, we are interested in a business intelligence dashboard to utilize our finance and shipping data to guide business decision making. We can do this by creating a story. 

1. Click **Create Your First Story**

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/1197ce5c47a4c2820bbfecb5590fa0fbbaa69a3c/exercises/ex1/images/Image%201.png)

Welcome to **Start Your Story Page! **
  
On this page, users can choose to import their own data, run a smart discovery on their data, add a responsive, canvas, or grid page, or start their story using a template. We are interested in exploring our data and the dimensions and measures we can analyze before we create a dashboard. 

2. Click **Responsive** 

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/e204a03413e854f5807a951718ca4f324924eae0/exercises/ex1/images/image%202.png)

<br> Let’s start by adding in some charts. 

3. Click **Insert** 

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/e55ed14b28058fb3f6e97a6880919a883d1bb21b/exercises/ex1/images/image%203.png)


4. Click **Chart**

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/Image%204.png)

<br> The data we will be using was already uploaded by a colleague in the Finance department. Let us access this model from the Public/TechEd folder in our tenant. 

5. Click **Public**

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/image%205.png)

6. Click **TechEd 2021**

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/image%206.png)

7. Click **ANA260_ORDER_FINANCE**

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/Image%207.png)

<br> Welcome to the Builder Panel!  
  
The Builder Panel is a place where you can create your visualizations. The chart area on your responsive page will remain empty until a measure and dimension are selected from the Builder Panel. It will dynamically update depending on the visualization that you are trying to create.  
  
We have just added an empty chart to our story and now we want to start adding measures and dimensions to build our chart into a visualization for business insights! 

8. Click **Add Measure**

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/image%208.png)

9. Scroll till you find **Sales Revenue**

10. Click S**ales Revenue**

11. Click Inside the Builder Panel to Collapse the Measure Selection Drop Menu

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/Image%209.png)

12. Click **Add Dimension **

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/Image%2012.png)

13. Scroll till you find **Region**

<br> Within the Dimension Selection Menu, a hierarchy icon is displayed next to hierarchaldimensions. Dimensions with attributes can be further expanded within the menu.

14. Click **Region**

15. Click Inside the Builder Panel to Collapse the Measure Selection Drop Menu

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/Image%2013_14_15.png)

<br> We have now created our first bar chart using the Builder Panel.

16. Resize the chart to be wider

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/Image%2016.png)
  
<br> **Quality Check!** Does our story page look like the screenshot? 

![alt text](https://github.com/SAP-samples/teched2021-ANA260/blob/main/exercises/ex1/images/Quality%20check%201.png)

<br> 17. We can easily change the layout of our story page. Click and drag the **Right Lane** to the **Top**

![Image 17](https://user-images.githubusercontent.com/90856848/137962398-4dc9b8ef-2e2c-48d4-a369-f3df0c8ec6e3.png)

<br>Let's start adding in some additional charts. First, we are interested in the gross margin breakdown across our different products. 

18. Click **Bottom Pane**

19. Click **Insert**

20. Click **Chart**

![Image 18_19_20](https://user-images.githubusercontent.com/90856848/137962472-35d808a8-e238-4808-8db7-201b076e9d2a.png)

<br> 21. Click **Add Measure** 

![Image 21](https://user-images.githubusercontent.com/90856848/137962592-6d198269-e592-4084-bfc3-661ee4abf92d.png)

<br>  22. Scroll to find **Gross Margin**

23. Click **Gross Margin**

24. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 22_23_24](https://user-images.githubusercontent.com/90856848/137962681-59f28b12-5321-40ac-b7ba-f65a0bb8ca13.png)

<br> 25. Click **Add Dimension**

![Image 25](https://user-images.githubusercontent.com/90856848/137962810-e03b2afe-d912-42a8-b210-a871d5b6829b.png)

<br> 
26. Scroll to find **Product**

27. Click **Product**

28. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu
 
![Image 26_27_28](https://user-images.githubusercontent.com/90856848/137962886-ade1a647-3b10-4220-bf89-e5d976fdf0a2.png)

<br> We have now created our second bar chart using the Builder Panel. However, our data can be further transformed to extract more valuable business insights. Let’s change the hierarchy level so we can see gross margin for different Product categories. 

![Image 28](https://user-images.githubusercontent.com/90856848/137963018-29d52182-8655-4584-a9bc-1626b64e82be.png)

<br> We can drill down on the Product dimension to get more information from our bar chart. You can also drill down on charts via the Builder Panel as a designer or by clicking on the bar and drilling down. 

29. Click **Set Drill**

30. Click **Level 2**

![Image 29](https://user-images.githubusercontent.com/90856848/137963173-5e36a339-0cd3-4196-9cdb-28e7b5b6b011.png)

<br> We can now see gross margin by each product category (Accessories, Clothing, Footwear), but we want to explore our data further and generate insights from the additional Workout Usage dimension in our model. 

![Image 30](https://user-images.githubusercontent.com/90856848/137963208-2777abee-6879-4e3f-9bdb-c3f4cf943c5c.png)

<br> 31. Under Color Click **+ Add Dimension/Measure**

![Image 31](https://user-images.githubusercontent.com/90856848/137967572-42c31ef3-dbf3-45bf-8e3f-b76feb85419d.png)

<br> 32. Scroll till **Workout Usage** is Visible

33. Click **Workout Usage**

34. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 32_33_34](https://user-images.githubusercontent.com/90856848/137967749-8966577b-f144-4498-8d49-dd9fe7955d9e.png)

<br> Our bar chart is now divided in each product category by its Workout Usage. Using Color in charts is an effective way of mapping additional dimensions into a visualization. We can change our Chart Type to better visualize the dimensions we have selected. 

![Image 34](https://user-images.githubusercontent.com/90856848/137967864-96b6bd25-6bb1-4697-8848-aaefaa83158d.png)

<br> 35. Click **Bar/Column Tile**

36. Click **Stacked Bar/Column**

![Image 35_36](https://user-images.githubusercontent.com/90856848/137967984-3f3ed97f-ddea-4545-ac4e-39bae787715d.png)

<br> We want to scale our chart so that the distribution of workout usage in each product category is easily comparable in percentages of the total. 

37. Click **Show Chart as 100%**

![Image 37](https://user-images.githubusercontent.com/90856848/137968133-4cb118f9-5244-455f-80bc-cbe1683ba0ea.png)

<br> 38. Resize the chart to be Wider

![image 38](https://user-images.githubusercontent.com/90856848/137968197-0e34f1e3-5d4f-490b-820a-5b8378d80db3.png)

<br> **Quality Check!** Does the Stacked Bar Chart in your story show up like this? 

Our chart visualization now displays for us the proportional distribution of gross margins in each Product Category based on their Workout Usage. This enables us to quickly analyze the contribution of the Workout Usage dimension within a Product Category

![Quality check 2](https://user-images.githubusercontent.com/90856848/137968340-b2bd3573-4608-445a-8d02-27cd2ae3a25d.png)

<br> We now want to analyze how our gross margin has been performing over time. Let us build a chart with a time dimension to display this data. 

39. Click **Insert**

40. Click **Chart**

![Image 39_40](https://user-images.githubusercontent.com/90856848/137968527-bff8353d-db89-48fb-a1bf-a3169ba45b77.png)

<br> 41. Click **+ Add Measure**

![Image 41](https://user-images.githubusercontent.com/90856848/137968639-5b3d1a68-b54a-4950-9042-8f42b5e18df9.png)

<br> 42. Scroll to find **Gross Margin**

43. Click **Gross Margin**

44. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 42_43_44](https://user-images.githubusercontent.com/90856848/137971075-57b51d61-83b1-4b69-9f4b-cc49bfe8bd2d.png)

<br> 45. Click **Add Dimension **

![Image 45](https://user-images.githubusercontent.com/90856848/137971191-06b7aa18-36d9-484e-a58a-507d2c685218.png)

<br> 46. Scroll to find **Order Date**

47. Click **Order Date**

48. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 46_47_48](https://user-images.githubusercontent.com/90856848/137971380-391f714e-5a91-451a-b638-a2ed7da77012.png)

<br> SAP Analytics Cloud immediately recognized our time dimension and created an upright chart orientation as per best practices. However, our chart currently shows an aggregation of all gross margins in our data set. Next, we want to apply a dynamic time filter for the year to date range and change the drill level to show months as the granularity of bars. 

![Image 48](https://user-images.githubusercontent.com/90856848/137971623-f2d9fba2-6b27-4423-9f48-e8b2089612b4.png)

<br> We have many options on filtering or drilling down on a dimension simply by hovering over the dimension in builder panel. 

49. Click **Filter** 

50. Click **Current**

51. Click **Year** under **To Date**

SAP Analytics Cloud offers users the ability to choose from a variety of dynamic time filters to quickly customize their charts to their business needs. We are using a year to date filter on our chart, so our data is filtered to begin on the start of the year 2021 until today. 

![Image 49_50_51](https://user-images.githubusercontent.com/90856848/137971814-bb2fd2ec-09d3-4511-987c-89231431b6b3.png)

<br> Let us Set Drill on our dimension. Currently our bar chart is aggregating data over all time, however we are more interested in seeing performance per month for the current year. 

52. Click **Set Drill**

Our hierarchy levels correspond to levels of granularity. In SAP Analytics Cloud, we dynamically provide various levels of time granularity (i.e. YQM, YHQM, YM). Currently, this chart is set to a YQM hierarchy with the first level set to aggregate over all time, so we want to select level 4 to reach monthly granularity

53. Click **Level 4**

![image 52_53](https://user-images.githubusercontent.com/90856848/137971995-18d6a306-27be-4be1-aca1-9e91cac54ade.png)

<br> We have just created a chart with a time dimension using a Year to Date filter to organize our visualization. Next, we want to learn more about the trend of Gross Margin from our chart. 
 
Please note your data will look different from this chart's values due to the dynamic date filter. 

54. Resize the chart to be wider

![Image 54](https://user-images.githubusercontent.com/90856848/137972097-afafbbfe-6d8a-452b-a8fe-2bb36d1274b6.png)

<br> We can look at the trend of Gross Margin from our chart by adding a trendline by using the context menu. 

55. Right Click on the chart to open the **Context Menu**

56. Click **Add**

57. Click **CGR (Compound Growth Rate)**

![Image 55_56_57](https://user-images.githubusercontent.com/90856848/137972267-afac9e7c-cc63-4cf9-80d2-b8b5d1a76135.png)

<br> We use the CGR added to the chart that compared to look at our compound growth rate in the year. If the CGR is negative it could be alarming information for the business user

![Image 57](https://user-images.githubusercontent.com/90856848/137972347-d430a655-fc5b-4c14-b3a1-31e5e137e1d5.png)






