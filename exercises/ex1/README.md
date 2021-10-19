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


