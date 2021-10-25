# Exercise 1 - Creating Your First Story

**Objective:** Develop a basic understanding on how to create visualizations within SAP Analytics Cloud. 

**Estimated Time:** 20 mins

**Exercise Description:** You want to visualize your company's performance over time, and find your first insights. 

**Key Features:**
- Understand how to use the Builder Panel
- Create a variety of different charts to illustrate key relationships within your data

⚠️**Disclaimer**
When completing exercises, some data values in the screenshots may not match what you see on your 
screen. This is because the dynamic time filters that were applied at the time the screenshots were taken is 
different from the current system date.

----------------------------------------------------------------------------------------------------------------------------------------

🚩As a business analyst for the BestRun company, we are interested in a business intelligence dashboard to utilize our finance and shipping data to guide business decision making. We can do this by creating a story. 

1. Click **Create Your First Story**

![Image 1](https://user-images.githubusercontent.com/90856848/138345550-bcaa9493-36dc-4dca-b148-04827f22dc2d.png)

<br> ℹ️Welcome to **Start Your Story Page!**
  
On this page, users can choose to import their own data, run a smart discovery on their data, add a responsive, canvas, or grid page, or start their story using a template. We are interested in exploring our data and the dimensions and measures we can analyze before we create a dashboard. 

2. Click **Responsive** 

![image 2](https://user-images.githubusercontent.com/90856848/138345633-6f60e8b2-01e4-4a76-8473-f7ac522420c2.png)

<br> 🚩Let’s start by adding in some charts. 

3. Click **Insert** 

![image 3](https://user-images.githubusercontent.com/90856848/138345734-9d5d535d-96ef-4120-b4b4-cb3076269197.png)

4. Click **Chart**

![Image 4](https://user-images.githubusercontent.com/90856848/138345773-f4008930-c87d-48a8-9e28-9b7fb92c912e.png)

ℹ️The data we will be using was already uploaded by a colleague in the Finance department. Let us access this model from the Public/TechEd folder in our tenant. 

5. Click **Public**

![image 5](https://user-images.githubusercontent.com/90856848/138345799-d9424d9d-93c1-4f92-a7a2-7b48e5e92a50.png)

6. Click **TechEd 2021**

![image 6](https://user-images.githubusercontent.com/90856848/138345832-b330da8a-01c2-4b32-a435-72cc196234d2.png)

7. Click **ANA260_ORDER_FINANCE**

![Image 7](https://user-images.githubusercontent.com/90856848/138345891-0f43ca72-86d0-4594-a7d6-bc44289a5b9e.png)

ℹ️Welcome to the Builder Panel!  
  
The Builder Panel is a place where you can create your visualizations. The chart area on your responsive page will remain empty until a measure and dimension are selected from the Builder Panel. It will dynamically update depending on the visualization that you are trying to create.  
  
We have just added an empty chart to our story and now we want to start adding measures and dimensions to build our chart into a visualization for business insights! 

8. Click **Add Measure**

![image 8](https://user-images.githubusercontent.com/90856848/138345940-634d5da3-6a22-4174-bb1f-7a4756e8b8d3.png)

9. Scroll untill you find **Sales Revenue**

10. Click S**ales Revenue**

11. Click Inside the Builder Panel to Collapse the Measure Selection Drop Menu

![Image 9](https://user-images.githubusercontent.com/90856848/138346008-0b98d4b3-d50e-42ce-abc9-61ed585a61f9.png)

12. Click **Add Dimension**

![Image 12](https://user-images.githubusercontent.com/90856848/138346155-7a8a9727-c156-4951-80fd-2325d3d28ba3.png)

13. Scroll untill you find **Region**

💡Within the Dimension Selection Menu, a hierarchy icon is displayed next to hierarchaldimensions. Dimensions with attributes can be further expanded within the menu.

14. Click **Region**

15. Click Inside the Builder Panel to Collapse the Measure Selection Drop Menu

![Image 13_14_15](https://user-images.githubusercontent.com/90856848/138346280-c19ab312-9ec8-40d2-a5d3-4e07c1e1897a.png)

🚩We have now created our first bar chart using the Builder Panel.

16. Resize the chart to be wider

![Image 16](https://user-images.githubusercontent.com/90856848/138346335-64195781-1b71-4273-9cb3-9a101aff8ea1.png)

⚠️**Quality Check!** Does our story page look like the screenshot? 

![Quality check 1](https://user-images.githubusercontent.com/90856848/138346373-46d6d074-c289-4291-9eca-644566236695.png)

17. We can easily change the layout of our story page. Click and drag the **Right Lane** to the **Top**

![Image 17](https://user-images.githubusercontent.com/90856848/137962398-4dc9b8ef-2e2c-48d4-a369-f3df0c8ec6e3.png)

🚩Let's start adding in some additional charts. First, we are interested in the gross margin breakdown across our different products. 

18. Click **Bottom Pane**

19. Click **Insert**

20. Click **Chart**

![Image 18_19_20](https://user-images.githubusercontent.com/90856848/137962472-35d808a8-e238-4808-8db7-201b076e9d2a.png)

21. Click **Add Measure** 

![Image 21](https://user-images.githubusercontent.com/90856848/137962592-6d198269-e592-4084-bfc3-661ee4abf92d.png)

22. Scroll to find **Gross Margin**

23. Click **Gross Margin**

24. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 22_23_24](https://user-images.githubusercontent.com/90856848/137962681-59f28b12-5321-40ac-b7ba-f65a0bb8ca13.png)

25. Click **Add Dimension**

![Image 25](https://user-images.githubusercontent.com/90856848/137962810-e03b2afe-d912-42a8-b210-a871d5b6829b.png)

26. Scroll to find **Product**

27. Click **Product**

28. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu
 
![Image 26_27_28](https://user-images.githubusercontent.com/90856848/137962886-ade1a647-3b10-4220-bf89-e5d976fdf0a2.png)

🚩We have now created our second bar chart using the Builder Panel. However, our data can be further transformed to extract more valuable business insights. Let’s change the hierarchy level so we can see gross margin for different Product categories. 

![Image 28](https://user-images.githubusercontent.com/90856848/137963018-29d52182-8655-4584-a9bc-1626b64e82be.png)

🚩We can drill down on the Product dimension to get more information from our bar chart. You can also drill down on charts via the Builder Panel as a designer or by clicking on the bar and drilling down. 

29. Click **Set Drill**

30. Click **Level 2**

![Image 29](https://user-images.githubusercontent.com/90856848/137963173-5e36a339-0cd3-4196-9cdb-28e7b5b6b011.png)

We can now see gross margin by each product category (Accessories, Clothing, Footwear), but we want to explore our data further and generate insights from the additional Workout Usage dimension in our model. 

![Image 30](https://user-images.githubusercontent.com/90856848/137963208-2777abee-6879-4e3f-9bdb-c3f4cf943c5c.png)

31. Under Color Click **+ Add Dimension/Measure**

![Image 31](https://user-images.githubusercontent.com/90856848/137967572-42c31ef3-dbf3-45bf-8e3f-b76feb85419d.png)

32. Scroll untill **Workout Usage** is Visible

33. Click **Workout Usage**

34. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 32_33_34](https://user-images.githubusercontent.com/90856848/137967749-8966577b-f144-4498-8d49-dd9fe7955d9e.png)

🚩Our bar chart is now divided in each product category by its Workout Usage. Using Color in charts is an effective way of mapping additional dimensions into a visualization. We can change our Chart Type to better visualize the dimensions we have selected. 

![Image 34](https://user-images.githubusercontent.com/90856848/137967864-96b6bd25-6bb1-4697-8848-aaefaa83158d.png)

35. Click **Bar/Column Tile**

36. Click **Stacked Bar/Column**

![Image 35_36](https://user-images.githubusercontent.com/90856848/137967984-3f3ed97f-ddea-4545-ac4e-39bae787715d.png)

🚩We want to scale our chart so that the distribution of workout usage in each product category is easily comparable in percentages of the total. 

37. Click **Show Chart as 100%**

![Image 37](https://user-images.githubusercontent.com/90856848/137968133-4cb118f9-5244-455f-80bc-cbe1683ba0ea.png)

38. Resize the chart to be Wider

![image 38](https://user-images.githubusercontent.com/90856848/137968197-0e34f1e3-5d4f-490b-820a-5b8378d80db3.png)

⚠️**Quality Check!** Does the Stacked Bar Chart in your story show up like this? 

🚩Our chart visualization now displays for us the proportional distribution of gross margins in each Product Category based on their Workout Usage. This enables us to quickly analyze the contribution of the Workout Usage dimension within a Product Category

![Quality check 2](https://user-images.githubusercontent.com/90856848/137968340-b2bd3573-4608-445a-8d02-27cd2ae3a25d.png)

🚩We now want to analyze how our gross margin has been performing over time. Let us build a chart with a time dimension to display this data. 

39. Click **Insert**

40. Click **Chart**

![Image 39_40](https://user-images.githubusercontent.com/90856848/137968527-bff8353d-db89-48fb-a1bf-a3169ba45b77.png)

41. Click **+ Add Measure**

![Image 41](https://user-images.githubusercontent.com/90856848/137968639-5b3d1a68-b54a-4950-9042-8f42b5e18df9.png)

42. Scroll to find **Gross Margin**

43. Click **Gross Margin**

44. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 42_43_44](https://user-images.githubusercontent.com/90856848/137971075-57b51d61-83b1-4b69-9f4b-cc49bfe8bd2d.png)

45. Click **Add Dimension**

![Image 45](https://user-images.githubusercontent.com/90856848/137971191-06b7aa18-36d9-484e-a58a-507d2c685218.png)

46. Scroll to find **Order Date**

47. Click **Order Date**

48. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 46_47_48](https://user-images.githubusercontent.com/90856848/137971380-391f714e-5a91-451a-b638-a2ed7da77012.png)

🚩SAP Analytics Cloud immediately recognized our time dimension and created an upright chart orientation as per best practices. However, our chart currently shows an aggregation of all gross margins in our data set. Next, we want to apply a dynamic time filter for the year to date range and change the drill level to show months as the granularity of bars. 

![Image 48](https://user-images.githubusercontent.com/90856848/137971623-f2d9fba2-6b27-4423-9f48-e8b2089612b4.png)

🚩We have many options on filtering or drilling down on a dimension simply by hovering over the dimension in builder panel. 

49. Click **Filter** 

50. Click **Current**

51. Click **Year** under **To Date**

🚩SAP Analytics Cloud offers users the ability to choose from a variety of dynamic time filters to quickly customize their charts to their business needs. We are using a year to date filter on our chart, so our data is filtered to begin on the start of the year 2021 until today. 

![Image 49_50_51](https://user-images.githubusercontent.com/90856848/137971814-bb2fd2ec-09d3-4511-987c-89231431b6b3.png)

🚩Let us Set Drill on our dimension. Currently our bar chart is aggregating data over all time, however we are more interested in seeing performance per month for the current year. 

52. Click **Set Drill**

🚩Our hierarchy levels correspond to levels of granularity. In SAP Analytics Cloud, we dynamically provide various levels of time granularity (i.e. YQM, YHQM, YM). Currently, this chart is set to a YQM hierarchy with the first level set to aggregate over all time, so we want to select level 4 to reach monthly granularity

53. Click **Level 4**

![image 52_53](https://user-images.githubusercontent.com/90856848/137971995-18d6a306-27be-4be1-aca1-9e91cac54ade.png)

🚩We have just created a chart with a time dimension using a Year to Date filter to organize our visualization. Next, we want to learn more about the trend of Gross Margin from our chart. 
 
⚠️Please note your data will look different from this chart's values due to the dynamic date filter. 

54. Resize the chart to be wider

![Image 54](https://user-images.githubusercontent.com/90856848/137972097-afafbbfe-6d8a-452b-a8fe-2bb36d1274b6.png)

🚩We can look at the trend of Gross Margin from our chart by adding a trendline by using the context menu. 

55. Right Click on the chart to open the **Context Menu**

56. Click **Add**

57. Click **CGR (Compound Growth Rate)**

![Image 55_56_57](https://user-images.githubusercontent.com/90856848/137972267-afac9e7c-cc63-4cf9-80d2-b8b5d1a76135.png)

🚩We use the CGR added to the chart that compared to look at our compound growth rate in the year. If the CGR is negative it could be alarming information for the business user

![Image 57](https://user-images.githubusercontent.com/90856848/137972347-d430a655-fc5b-4c14-b3a1-31e5e137e1d5.png)

🚩Let us add a table to our story to examine our Gross Margin contribution by each Sales Manager. Since Sales Manager is a high cardinality dimension with a lot of members, it is recommended to view this data in a table. 

58. Click **Insert** 

59. Click **Table**

![Image 58_59](https://user-images.githubusercontent.com/90856848/137972974-0195f8b2-8ee2-40e9-b2e6-ac3e3ff1f741.png)

60. Under **Rows** Click **+ Add Measures/Dimensions**

![Image 60](https://user-images.githubusercontent.com/90856848/137977280-1e94e91b-9ac1-4617-aded-d50bc9abdebb.png)

61. Scroll untill **Product** and **Sales Manager** is visible

62. Click **Product**

63. Click **Sales Manager**
 
64. Click inside the Builder Panel to Collapse the Measure/ Dimension Selection Drop Down Menu

![Image 61_62_63_64](https://user-images.githubusercontent.com/90856848/137977475-e14757f7-800e-43c9-8b11-592c01d2a82d.png)

🚩We can see that a table has been created to track Sales Managers. We can choose to expand the Product column to sort our table by Product Category contributions by each Manager. However, our table measure is currently set to Discount. Let’s change it to Gross Margin. 

![Image 64](https://user-images.githubusercontent.com/90856848/137977602-5ee0a1ae-bf2a-4bcb-8fb9-72dbc793be6a.png)

65. Return to the Builder Panel. Click **Filter** on Account Column

![Image 65](https://user-images.githubusercontent.com/90856848/137977680-0a2bbc52-85f9-4d19-81a5-5662e48dba80.png)

66. **Deselect Discount**

67. Select **Gross Margin**

68. Click **OK**

![image 66_67_68](https://user-images.githubusercontent.com/90856848/137977807-3c040055-e028-4849-baad-9dee3aa85fff.png)

🚩We have created a table to show contributions of Sales Manager to Gross Margin; however, this value is an aggregate over the entire period spanning the model. We would like to breakdown on Order Date to better interpret the yearly contributions of each Sales Manager to 
Gross Margin 

![Image 68](https://user-images.githubusercontent.com/90856848/137977889-82e2fef3-063f-4512-858f-6644f5f06728.png)

69. Under **Columns** Click **+ Add Measures/Dimensions**

![Image 69](https://user-images.githubusercontent.com/90856848/137977994-c55411e2-86a8-45ef-a40f-bc397e3e9bc7.png)

70. Scroll untill Order Date is Visible

71. Click **Order Date**

72. Click inside the Builder Panel to Collapse the Measure/ Dimension Selection Drop Down Menu

![Image 70_71_72](https://user-images.githubusercontent.com/90856848/137978113-fd5b3b06-d6ab-4ad1-bfea-20b3fb233868.png)

⚠️**Quality Check!** Does your table have the Product, Sales Manager, and Gross Margins columns? 

🚩There has been an Order Date field added to our table. If we expand on all, Gross Margin will be separated into yearly sums. We want to see our Gross Margin % in our table but we currently do not have that measure in our data model. We can create the Gross Margin % measure as a calculation with the Sales Revenue and Gross Margin measures

![Quality Check 3](https://user-images.githubusercontent.com/90856848/137978245-4ac60fa9-c59f-41bb-a004-a24999f17150.png)

🚩We may be looking for more insights from our data and can do so by creating a calculation! 

73. Click the **More** Icon for Account

74. Click **Add Calculation**

![Image 73_74](https://user-images.githubusercontent.com/90856848/137978372-38974189-aca5-471d-8fe7-fca367f1da87.png)

ℹ️Welcome to the Calculation Editor! 
  
The Calculation Editor allows you to create calculations for use in a chart or table. There are various types of calculations that a user can create which include:  
  
1. **Calculated Measures**: Perform a  calculation on one or more measures

3. **Restricted Measures**: Restrict the data from a measure so that it excludes certain members of one or more dimensions  

5. **Difference From**: Find the difference in a measure's value between two points in time for a single time dimension  
 
4. **Aggregation**: Create an aggregation such as sum, count, count dimensions, max, and max  
  
5. **Date Difference**: Calculate the difference between two-time dimensions  
  
6. **Dimension to Measure**: Create a measure by converting a dimension to measure. 

We will cover calculations in more detail for business analytics use cases in our **Section 7 - Calculations and Blending Deep Dive**. You can jump off to this section to learn more. 

![Image 74](https://user-images.githubusercontent.com/90856848/137978728-f825539c-015a-4480-9c15-fc48b5a2230b.png)

75. Click **Calculated Measure**

![Image 75](https://user-images.githubusercontent.com/90856848/137978876-a1f5e2ff-680d-4acc-b26b-05adabcf321a.png)

76. Click the formula field and enter **"gro"**

77. Click **["ANA260_ORDER_FINANCE": Gross_Margin]**

![Image 76_77](https://user-images.githubusercontent.com/90856848/137979038-613f7fcf-093d-4c87-8ae0-a1d7f7c76e6e.png)

78. Type in **"/"** to indicate we want to divide in our calculation

79. Type in **"Sal"**

80. Click **["ANA260_ORDER_FINANCE":Sales_Revenue]**

![Image 78_79_80](https://user-images.githubusercontent.com/90856848/137979177-9ac3a396-215f-49f0-b63c-31b4211d7f65.png)

81. Name the measure **Gross Margin %**

82. Click **OK**

![image 81_82](https://user-images.githubusercontent.com/90856848/137979310-1d12cb34-c7d6-4fb5-9283-5b0b0b8c6e67.png)

🚩Now let’s use our newly made calculation in our table and remove the previous measure. 

83. Click **Filter** on Account in Columns

![image 83](https://user-images.githubusercontent.com/90856848/137989991-811df258-030d-4a46-93e4-e3b6fc57b818.png)

84. Deselect **Gross Margin**

85. Click **OK**

![Image 84_85](https://user-images.githubusercontent.com/90856848/137990159-b5f17322-b34f-4880-89c2-af42b0b9d27f.png)

🚩Now that we have our desired measure, let’s expand the Order Date column to see our values on a yearly basis. 

86. Click **> (All)** to Expand the Order Date Dimension

![image 86](https://user-images.githubusercontent.com/90856848/137990257-64901f37-9ad8-411f-88d0-c708a6314080.png)

🚩We want to hide the all column that aggregates Gross Margin %. 

87. Right Click the **All Order Date Column**

88. Click **Hide Column**

![Image 87_88](https://user-images.githubusercontent.com/90856848/137990379-2df94ee6-2b7b-4476-9ef6-e98c27f14531.png)

🚩Our table should look like this screenshot now. Since our calculation is a percentage, we will now change the formatting of our values to improve our table visualization. 

![Image 88](https://user-images.githubusercontent.com/90856848/137990473-4703cc71-5fb0-442e-8ede-4d82fb4b50bf.png)

🚩We can easily change the formatting and representation of our measures and calculations. 

89. Click **Story Calculations**

90. Click **Formatting**

![Image 89_90](https://user-images.githubusercontent.com/90856848/137990609-6e7e78c5-0caa-4f38-aadf-b879be1f8bda.png)

91. Deselect **Use Unit of Underlying Measures**

92. Change Scale to **Percentage**

93. Change Decimal places to 0

94. Click **OK**

![Image 91_92_93_94](https://user-images.githubusercontent.com/90856848/137990847-9feb9649-7bc3-430b-a24f-ff22e8bd88fe.png)

⚠️**Quality Check!** Does our table look like this screenshot? We have now formatted our chart so the % symbols for gross margin are indicated in the subtitle. This cleans up the table visualization. 

![Quality Check 4](https://user-images.githubusercontent.com/90856848/137991025-72a18c2f-ed54-44cb-b280-468ec84aaff3.png)

🚩Let us shift our focus back to our dashboard layout. We want to now add some KPIs that stand out for story viewers. 

95. Select **Top Lane**

![Image 95](https://user-images.githubusercontent.com/90856848/137991131-0f38faa3-82b3-4a70-83ce-adbe5ae0cc56.png)

🚩Since this lane is in now at the top of our dashboard, let us add some easily viewable KPIs as numeric point charts in our story. Numeric point charts are a chart visualization that display the total of a measure and are best suited for highlighting key business KPIs. They can be filtered so the KPI describes a specific context relevant to the business user. 

96. Click **Insert**

97. Select **Chart**

![Image 96_97](https://user-images.githubusercontent.com/90856848/137991293-6d1655d1-60c9-458b-90fc-642a4710131f.png)

98. **Click Target**

99. **Click Numeric Point**

![Image 98_99](https://user-images.githubusercontent.com/90856848/137993390-7e14db61-a527-418d-9cd0-a5e661934121.png)

100. Click **Add Measure**

![Image 100](https://user-images.githubusercontent.com/90856848/137993462-8908f81b-9664-40b7-9bb5-dccb70cb9bb8.png)

🚩Let us use Gross Margin as our first KPI. 

101. Scroll untill Gross Margin is visible

102. Click **Gross Margin**

103. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 101_102_103](https://user-images.githubusercontent.com/90856848/137993553-d6dd7fc7-b4fe-4617-bfea-f6d9bb2fdd07.png)

🚩We should add a date filter on our KPI, so the context is more relevant to a business analyst looking for actionable insights. Let us filter data for the current year. 

104. Click **Add Filters**

![image104](https://user-images.githubusercontent.com/90856848/137993674-81bc10dd-13d5-45e3-891a-191417334e3a.png)

105. Click **Order Date (Member)**

![Image 105](https://user-images.githubusercontent.com/90856848/137993790-445062df-c582-4001-b84a-61c4a8c2eb8e.png)

106. Click the **Expand** icon

107. Click **2021**

108. Click **OK**

![Image 106_107_108](https://user-images.githubusercontent.com/90856848/137994376-8e64baa4-0818-4fb0-ab82-3b8f24ab1b79.png)

🚩You have now created a numeric point chart that displays Gross Margin filtered for only data in 2021. 

109. Decrease the size of the Numeric Point Chart

![Image 109](https://user-images.githubusercontent.com/90856848/137994450-af633095-8423-449a-925a-e22706f2aa9b.png)

🚩Let us use SAP Analytics Cloud's duplicate chart functionality to easily create our other KPIs. 

110. Click the **More** icon

111. Click **Copy**

112. Click **Duplicate**

![Image 110_111_112](https://user-images.githubusercontent.com/90856848/137994536-93b59d50-dd2c-4f0f-abac-17d38569057d.png)

⚠️**Quality check!** Has your dashboard updated with a copied KPI chart like this screenshot? 

![Quality Check 5](https://user-images.githubusercontent.com/90856848/137994604-f78ff270-2a04-4c99-9556-89d3382d205c.png)

ℹ️We want to create a new KPI of Sales Revenue like our first chart of Gross Margins. Since we duplicated the KPI, our previously applied date filter will be automatically applied to our new KPI. Let us now change the measure of our second KPI. 

113. Deselect the Gross Margin measure for your new chart by clicking **Remove**

114. Click **Add Measure**

![Image 113_114](https://user-images.githubusercontent.com/90856848/137994720-c71681d7-6171-4190-ac11-dc0a7cf95ba9.png)

115. Scroll until **Sales Revenue** is visible

116. Click **Sales Revenue**

117. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down Menu

![Image 115_116_117](https://user-images.githubusercontent.com/90856848/137994817-313c1585-f8da-4d4d-ab9b-a2a7a09aad98.png)

🚩Now that we are satisfied with our second KPI for Sales Revenue, let us duplicate this chart again to create a KPI that calculates average sales revenue. 

118. Click the **More** icon

119. Click **Copy**

120. Click **Duplicate**

![Image 118_119_120](https://user-images.githubusercontent.com/90856848/137994876-ff3c9657-4fec-49e3-a60e-de5c531b3c4c.png)

🚩We currently do not have a measure for our average sales revenue by store in our model. Hence, let us create a calculation to track this metric on our dashboard. 

121. Remove Sales Revenue as a Measure

122. Click **Add Measure**

![Image 121_122](https://user-images.githubusercontent.com/90856848/137994960-6515a7c9-5632-4e72-8f66-8d1df87a6212.png)

123. Click **Create Calculation** in **Add Measure**

![Image 123](https://user-images.githubusercontent.com/90856848/137995024-c34a8f38-e1cb-42ae-9d0d-405cc9266b62.png)

🚩We want to calculate the average sales revenue by store for our company. This will require an aggregation of all sales revenue averaged by number of stores. We can create this in the Aggregation Calculation Type. 

124. Select **Aggregation** as Calculation Type

![Image 124](https://user-images.githubusercontent.com/90856848/137995115-e628f923-c48b-4336-b88c-5560d32d4b27.png)

125. Click **Expand** for **Operation**

126. Scroll till AVERAGE is Visible

127. Click **AVERAGE**

![Image 125_126_127](https://user-images.githubusercontent.com/90856848/137995225-83e32c59-4229-43f9-aebb-896db54fc98a.png)

128. Click **Expand** for **Operation**

129. Click **Sales Revenue**

![Image 128_129](https://user-images.githubusercontent.com/90856848/137995377-00b912c4-7dcb-49f3-89f9-c28118bbf2b3.png)

🚩Here we are selecting the aggregation dimension that will be used to calculate our average. Since we want average sales revenue by store, we should change this dimension to Store. 

130. Click **Expand** for **Aggregation Dimensions**

131. Scroll till Store is Visible

132. Click **Store**

![Image 130_131_132](https://user-images.githubusercontent.com/90856848/137995484-d37e28c3-9d5b-46bb-9349-b7a74feea345.png)

133. Rename the calculation to **Avg Sales Revenue**

134. Click **OK**

![Image 133_134](https://user-images.githubusercontent.com/90856848/137995657-dee75c9b-8f79-49f1-8caa-b0f73f49b3cc.png)

⚠️**Quality Check!** Do your numeric point charts have these values and measures on your story? Please note that your time chart may look different from this screenshot due to the dynamic date filter on YTD. 

![Quality Check 6](https://user-images.githubusercontent.com/90856848/137995743-a107a55f-1b68-4241-a7dd-42667a22950a.png)

🚩At this stage, you should save your first story. 

135. Click **File** 

136. Click **Save**

137. Click **Save**

![Image 135_136_137](https://user-images.githubusercontent.com/90856848/137997594-45a05e2c-e770-4a06-9e5c-c138748d9844.png)

137. Save your story in My Files as **ANA260_ Your Initials**

138. Click **OK**

![Image 138_139](https://user-images.githubusercontent.com/90856848/137997679-c3218706-0bc8-43bd-ada2-5f80ebc37221.png)

🚩 You can also save your story by pressing **Ctrl + S** on your keyboard

![Image 139](https://user-images.githubusercontent.com/90856848/137997730-de780fc1-a9a3-41c2-bf0b-2bacdf70c955.png)

ℹ️You have completed **Creating Your First Story!** 
  
Please continue with the next section **Linked Analysis and Input Controls**. We will also improve the styling of this dashboard in **Section 4 - Theme and Style!**

![Final Picture](https://user-images.githubusercontent.com/90856848/137997823-ed675788-ac8a-4c9a-9ddc-3c3a0795dd54.png)

<br><br>



## Summary

**You have completed the entire Create Your First Story section!**

**You are now able to:**
- Understand how to use the Builder Panel
- Create a variety of different charts to illustrate key relationships within your data


