# Section 3 - Geo Maps, Thresholds, and Variance

ℹ️Welcome to the **Geo Maps, Thresholds and Variance** section! We will also go into greater detail on the analytic capabilities available to story creators with geo maps and geo-enriched data in our **Section 8 - Geo Visualizations Deep Dive**. 
 
Exercise check! Does your dashboard look like this screenshot? 

![3-1](https://user-images.githubusercontent.com/92877810/138260047-5b7838cf-581e-4a86-a6a0-8a4c4f0b9425.png)

🚩Let us start by adding some geographical information into our dashboard. 

1. Click **Insert**

2. Click **Geo Map**

![3-2](https://user-images.githubusercontent.com/92877810/138260049-7ffbb9bb-7abd-425d-9069-39ca7a288e74.png)

⚠️Quality check! Does a geo map appear at the bottom right of your dashboard like this screenshot? Does the Builder panel open with your geo map selected? 

![3-3](https://user-images.githubusercontent.com/92877810/138260051-4ecc4fda-699e-4271-a5ff-d23e9cdd07db.png)

🚩Geo visualizations consist of one or multiple layers which can be sourced from different data sets. For our purposes, we will be using a bubble layer to individually represent measure values at store coordinates. 

3. Click **+ Add Layer**

![3-4](https://user-images.githubusercontent.com/92877810/138260052-c4f2d99b-7b7b-4a6a-89be-93ea722436c0.png)

🚩We are going to be using a secondary model in this exercise. SAP Analytics Cloud supports using multiple models in a dashboard to best represent your story. Let us swap to our shipping model so we can display average delivery times by country in our geo map. 

4. Click **Select Model**

![3-5](https://user-images.githubusercontent.com/92877810/138260053-507e3619-6d00-463e-8ecd-7e5c20722133.png)

5. Click **Select Other Model...**

![3-6](https://user-images.githubusercontent.com/92877810/138260055-4d81c8c7-1758-47e1-ae54-fb351b037842.png)

6. Click **Public**

![3-7](https://user-images.githubusercontent.com/92877810/138260056-c6ee6d2f-e9aa-4cdf-a3f1-03b33be74531.png)

7. Click **TechEd 2021**

![3-8](https://user-images.githubusercontent.com/92877810/138260057-7a796520-f0ec-437a-ae32-592a4231b91f.png)

8. Click **ANA260_SHIPPING_INFO**

![3-9](https://user-images.githubusercontent.com/92877810/138260058-8d7a5e9c-1dd6-4b6e-9af3-35f79e0a9521.png)

9. Click **Add Location Dimension**

![3-10](https://user-images.githubusercontent.com/92877810/138260059-f48c47ca-65b7-496a-96c5-c35140cc718b.png)

🚩The dimension displayed in Location Dimension is a geo-enriched dimension that can be built in your dataset from location names or latitude/longitude coordinates. 

10. Click **StoreLocation**

![3-11](https://user-images.githubusercontent.com/92877810/138260785-182f29d8-45fd-47c4-9432-bd954c358bf2.png)

⚠️Quality Check! Does your Geo Map populate with stores like this screenshot? 

🚩Let us color our bubbles based on average delivery time so we can easily see which locations are taking longer to receive deliveries.

![3-12](https://user-images.githubusercontent.com/92877810/138260788-bef29639-0489-4d12-b9ea-f5a81f327ee0.png)

11. Click **+ Add Measure/Dimension**

![3-13](https://user-images.githubusercontent.com/92877810/138260790-0ca830f6-d835-4991-8709-b0825490e69c.png)

🚩Let us select average delivery time to color code our bubbles so we can identify which stores are receiving deliveries slower. 

12. Click **Avg Delivery Time**

![3-14](https://user-images.githubusercontent.com/92877810/138260791-1d7027a3-9b67-4b4a-ae3e-f59d841bcc3c.png)

⚠️Quality check! Does your geo map look like this screenshot? Next, we will look at using a different layer type to represent our data. 

![3-15](https://user-images.githubusercontent.com/92877810/138260792-abab03c4-3b01-47dd-b6d0-f5d2117228ea.png)

🚩There are other layers applicable to our 
Geo Map. Let us look at average delivery time aggregated based on location rather on an individual store level. We can do this by choosing to add a choropleth layer. We will go into further detail on the other layer types available in SAP Analytics Cloud in our **Section 8 - Geo Visualizations Deep Dive** section. 

13. Click **Expand** for **Layer Type**

14. Click **Chloropleth/ Drill Layer**

![3-16](https://user-images.githubusercontent.com/92877810/138260793-5ea01bb8-cf4f-4d2e-be62-6f9ee2433ee1.png)

ℹ️A choropleth layer aggregates values in the Geo Map, making it easier for a user to discover outliers and trends. As we can see in the geo visualization, Spain appears to have higher than average delivery times on orders. Let’s drill down on this layer to understand the data. 

15. Click on **Spain**

![3-17](https://user-images.githubusercontent.com/92877810/138260795-64a9371f-0cce-427e-a879-06fe6c42cdf0.png)

ℹ️When we click on Spain, we get a context menu with options to Drill down or up on the hierarchy level as well as filter on or exclude Spain's data from the geo map. We want to look at regional average delivery times in Spain so let us drill down on this hierarchy. 

16. Click **Drill Down**

![3-18](https://user-images.githubusercontent.com/92877810/138260796-bbf023d8-7f53-4765-9095-93630ef6d8d0.png)

ℹ️From drilling down on our country layer, we are now able to see the distribution of average delivery times in the regions of Spain. It appears only one region is doing poorly and may require further business action. Let’s return to our country layer. 

17. Click **Drill Filter**

18. Click **Remove**

![3-19](https://user-images.githubusercontent.com/92877810/138260798-22695941-29db-43fa-a263-fb16718c2dcc.png)

⚠️Quality check! Does your geo map now look like this screenshot? 

![3-20](https://user-images.githubusercontent.com/92877810/138260799-1b3045eb-3ab4-407e-bf96-f5b28ced95bd.png)

ℹ️Up to this point, we have created a lot of visualizations. For us to easily draw conclusions and highlight key insights, we should add variances and thresholds on our charts in our dashboard so we can draw attention to changes and outliers. 

![3-21](https://user-images.githubusercontent.com/92877810/138261811-ccb46f24-2b2e-44cd-bc9f-65e5babceb12.png)

🚩First, let us add a variance to our KPI for average sales revenue in stores so we can compare if average sales revenue has dropped this year relative to our previous year's performance. If you can recall, our KPIs currently have a 2021 time filter applied on them. 

19. Right Click on the Avg Sales Revenue Chart to Open the Context Menu

20. Click Compare To

21. Click Previous Period

🚩We want to compare our data in 2021 year to date with the calculation for the previous year. By comparing to previous period, SAC will automatically calculate this variance for us. 

![3-22](https://user-images.githubusercontent.com/92877810/138261815-181434bd-67c1-4f37-b97e-b6319df2c378.png)

🚩After creating our variance, the absolute value may still be hard to contextually understand. We want to know the percentage difference so let us edit this variance. 

![3-23](https://user-images.githubusercontent.com/92877810/138261816-7eaefbe5-59b2-4fe0-b0ae-aa4dd3d848a3.png)

22. Click **1 Variance**

23. Click **Edit All Measures in Use**

![3-24](https://user-images.githubusercontent.com/92877810/138261817-c5304eab-976e-4c15-b1dc-fcd2913ff093.png)

🚩In this panel, users can choose how they want to format their variances to best fit their data. We are comparing a KPI across two periods using a single number. In this instance, a percentage would be easier to understand for an end user. 

24. Click **Percentage**

25. Deselect **Numbers**

26. Click on **Avg Sales Revenue for Actual** to Collapse the Variance Panel

![3-25](https://user-images.githubusercontent.com/92877810/138261818-9c84e36a-6eeb-45ff-a5db-4a508521d031.png)

🚩The new variance looks great! We can now clearly see that average sales revenue in our stores has experienced a 3.7% drop from the last period. 

![3-26](https://user-images.githubusercontent.com/92877810/138261820-4d487ce7-79be-4bd8-ab9a-53445779ee16.png)

🚩Now let’s add more variances to our chart. A good candidate to track change in data over time is our chart using a time dimension. SAC offers recommended comparisons in the builder panel as a suggestion for easy creation of variances. 

27. Select your **Gross Margin per Order Date for Actual** Chart

🚩We want to select Previous Period because it will dynamically change the variance based on the granularity in the chart. 

28. Expand **Recommened Comparisons**

29. Click **Previous Period**

![3-27](https://user-images.githubusercontent.com/92877810/138261821-154f9835-dac8-4f7a-9d40-d52f19f718a8.png)

🚩Our variances show the delta to the period before, in this case the last month's gross margin. We want to know the percentage difference instead of absolute difference. Let us change the formatting of our variance values. 

![3-28](https://user-images.githubusercontent.com/92877810/138261822-434fb259-be1f-43b8-8ddf-a193366b87f5.png)

30. Scroll to the Bottom of the Builder Panel

31. Click **Edit** for the Variance **All Measure in Use (Previous Period)**

![3-29](https://user-images.githubusercontent.com/92877810/138261823-27ca40d7-c623-4e1e-abe8-c71544e5991d.png)

32. Expand **Display Options**

33. Scroll to the Bottom of the Builder Panel

34. Click **Percentage**

35. Deselect **Numeric**

36. Click **OK**

![3-30](https://user-images.githubusercontent.com/92877810/138261824-2f15a39e-296d-4582-9601-a83dc45fb56f.png)

⚠️Quality check! Have your variances in the chart updated to percentage values? Please note your data will look different due to the dynamic time filter on the chart

![3-31](https://user-images.githubusercontent.com/92877810/138261825-3b5fffe4-a935-4968-b6ff-e73fe5248003.png)

🚩Let’s alter this chart so it is easier to compare Sales Managers. We can sort the chart and create a dynamic reference line to benchmark individual Sales Managers against the average. 

37. Right Click the **Gross Margin per Sales Manager per Actuals** Chart to Open the Context Menu

38. Click Sort

39. Click **New Measure Input Control**

40. Click **Highest to Lowest**

![3-32](https://user-images.githubusercontent.com/92877810/138261826-c71bb5c7-c73e-437e-9479-6d1f2e364c26.png)

⚠️Quality check! Is your chart now sorted in descending order for the selected measure? If we chose to swap gross margin for sales revenue in the measure input control, our chart would re-sort itself in descending order corresponding to the new measure. 

![3-33](https://user-images.githubusercontent.com/92877810/138261828-bc760507-e052-43d0-8c46-e766139b59c5.png)

🚩Let us add a benchmark to compare our sales manager performances with the average gross margin per sales manager

41.  Right Click the **Gross Margin per Sales Manager per Actuals** Chart to Open the Context Menu

42. Click **Add**

43. Click **Reference Line**

![3-34](https://user-images.githubusercontent.com/92877810/138261831-306d5315-66d6-4390-942b-c9e778dad47a.png)

🚩We want to create a dynamic reference line so that our benchmark will update with the selected measure given by our measure input control. 

44. Click **Dynamic** in the Panel for Create Reference Line

45. Click **Select Measure**

46. Expand **ANA260_ORDER_FINANCE**

ℹ️By choosing a Measure Input Control as the measure for the reference line, any changes to the input control will be reflected in a new reference line. 

47. Click **Measure Input Control** as measure for calculating reference line

48. Click **OK**

![3-35](https://user-images.githubusercontent.com/92877810/138261832-71ff76c5-4d49-4676-8714-b23d879095b0.png)

⚠️Quality Check! Do you have a reference line and sorted chart for Sales Managers in your story? 

![3-36](https://user-images.githubusercontent.com/92877810/138261833-dc632fc6-6eb0-426c-aea1-ad536339beee.png)

🚩We would like to now add a variance in our table to easily highlight the change in gross margin % between years. This can be done automatically through the context menu. 

49. Select the columns 2020 and 2021 in the Table

50. Right Click to Open the Context Menu

51. Click **Add Column**

52. Click **Single**

![3-37](https://user-images.githubusercontent.com/92877810/138261834-7e46845c-1b63-4751-9957-7d6956ef8007.png)

🚩A new column has been created that represents the differences in values between 2019 and 2020. We want to add a visual indicator to see whether our delta is below or above the previous year. 

53. Right Click on Delta to Open the Context Menu

54. Click **Thresholds**

55. Click **New Threshold...**

![3-38](https://user-images.githubusercontent.com/92877810/138261835-64e1854b-f811-4b08-bd52-9fa25c6dcf87.png)

ℹ️Welcome to the Thresholds panel. 
  
Within Thresholds, you can create a threshold based on a number range or against another measure. In our case, we are interested in a number range. 

56. In Threshold Panel, Click **Add Range**

![3-39](https://user-images.githubusercontent.com/92877810/138261836-4316999f-d492-4fdc-9ff9-9484a2f432d8.png)

57. Enter 0 for the OK (Green) Min Range

58. Enter 0 for the Warning (Yellow) Max Range

![3-40](https://user-images.githubusercontent.com/92877810/138261837-a00d7b3c-1e41-4827-876d-eca788fb49c9.png)

59. Expand the **Orange Indicator**

60. Choose the **Red Indicator**

61. Click **Apply**

![3-41](https://user-images.githubusercontent.com/92877810/138261839-55e6ab20-3a6d-4dba-9587-d14462d58392.png)

🚩Users can see by scrolling through the table that an appropriate indicator has been given to values in each threshold in the Delta column. 
  
We would like to change how this value is displayed to only highlight the number rather than adding an indicator. 

![3-42](https://user-images.githubusercontent.com/92877810/138261840-30de12bd-f485-4d8d-99e6-b9915487e5e4.png)

62. Click **Designer** to Open Builder Panel (in case not already open)

63. Click **Styling**

![3-43](https://user-images.githubusercontent.com/92877810/138261841-a745789d-f862-43a1-ba58-03c933ce00f0.png)

ℹ️Welcome to the Styling Panel! 
  
The Styling Panel displays options available for the selected tile type. Some options may not be available to all users.  
  
For widget, you see only the styling options for the specific area that you have highlighted. The heading in the Styling Panel identifies the area. For example, it may show Title, Data Cell, Axis Labels, and so on. Selecting a different part of the widget changes the heading and the styling options. 

![3-44](https://user-images.githubusercontent.com/92877810/138261842-9bb75e2e-26fb-4c78-87b7-622c4102c5b9.png)

64. Expand **Threshold Style**

65. Click **Color Values**

![3-45](https://user-images.githubusercontent.com/92877810/138261843-bcf22ea7-26f3-42e8-8474-88e795adde2b.png)

🚩Thresholds in the table are now color coded instead of representation by a symbol indicator. 

![3-46](https://user-images.githubusercontent.com/92877810/138261844-ccf89b5c-0321-4451-aeed-29d15cd5418b.png)

⚠️Quality Check! Does your dashboard with thresholds and variances look like this screenshot? 

🚩Please save your story by pressing **Ctrl + S** on your keyboard! 

![3-47](https://user-images.githubusercontent.com/92877810/138261847-1706de9d-af06-4c1b-8774-3a19f90ef649.png)

ℹ️You have now completed the **Geo Maps, Thresholds, and Variances** section! In this section we learned how to create geo visualizations to populate our dashboard, add thresholds, dynamic reference lines, and variances to our charts to highlight key insights.
  
To explore more of SAP Analytics Cloud's capabilities in analyzing geo enriched data, you can jump off to **Section 8 - Geo Visualizations Deep Dive**. 
 
![3-48](https://user-images.githubusercontent.com/92877810/138261848-de24c692-62f2-410a-be46-a70b2c52d1b4.png)

