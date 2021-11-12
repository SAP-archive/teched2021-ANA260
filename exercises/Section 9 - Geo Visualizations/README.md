# Section 9 - Geo Visualizations Deep Dive

ℹ️**Objective:** Use Geo Maps in SAP Analytics Cloud to interpret geo-enriched models and enhance your 
dashboard’s analytic capabilities. Develop an understanding of the various features available in geo 
visualizations to customize your insights.

**Estimated Time:** 20 mins

**Exercise Description:**  You need to do a deeper analysis on BestRun’s regions and understand what drives 
geographical differences in the company’s performance. You need to leverage geo-spatial analytic 
capabilities of SAP Analytics Cloud to create new geo maps for your analysis.

**Key Features:**
- Create your own geo-enriched models with acquired data
- Employ heat maps to gather insights on geo data density
- Understand the use of distance filters and the lasso tool in analyzing your hypotheses
- Use tooltips, labels, and overlapping points to enhance the insights in your geo map
- Change your basemap layer to view your geo enriched data in different contexts
- Style your geo map for clear and informative visualizations

⚠️**Disclaimer**
When completing exercises, some data values in the screenshots may not match what you see on your 
screen. This is because the dynamic time filters that were applied at the time the screenshots were taken is 
different from the current system date.

----------------------------------------------------------------------------------------------------------------------------------------

⚠️**Excercise Check!** Does your story look like this? 

![9-1](https://user-images.githubusercontent.com/92877810/139945745-2f9ecdfa-81de-4a0e-aacd-b1e907adb605.png)

1. Click **Files**

![9-2](https://user-images.githubusercontent.com/92877810/139945749-c85a8850-3c1f-4bfc-801b-90b20f64e4ae.png)
  
🚩If you are not in the TechEd 2021 folder, follow the path: **Public/TechEd 2021**

2. Select **Section 9.0 - Geo Visualizations(Start)**

3. Click Copy To

![9-3](https://user-images.githubusercontent.com/92877810/139945752-a12e1bb3-d478-4fef-b7e4-b5e5b7357a4f.png)

4. Click **MyFiles**

![9-4](https://user-images.githubusercontent.com/92877810/139945754-9aa48c78-2b6e-4573-8971-bf2ffefb0083.png)

5. Save the file in MyFiles under the name **"ANA260_Section 9_Your Initials"**

6. Click **OK**

![9-5](https://user-images.githubusercontent.com/92877810/139945756-a42f10c7-5571-473f-931a-c29f479a2565.png)

7. Click **MyFiles**

![9-6](https://user-images.githubusercontent.com/92877810/139945757-7f017c9d-4d54-410d-8bb4-d5e6f2aa1357.png)

8. Open **ANA260_Section 9_Your Initials** file 

![9-7](https://user-images.githubusercontent.com/92877810/139945758-13b8af2e-4546-4cd4-8c72-37334772ed2e.png)

9. Click **Edit**

![9-8](https://user-images.githubusercontent.com/92877810/139945760-813d6eea-3c5d-4bee-93e1-5b5b94f0188e.png)

10. Click **Shipping Analysis** Page 

![9-9](https://user-images.githubusercontent.com/92877810/139945762-2071c6e1-c750-429d-8df8-ff75d61ae171.png)

ℹ️Excercise Check! Does your dashboard look like this screenshot? 

![9-11](https://user-images.githubusercontent.com/92877810/139945767-3b948ba2-6e6c-4592-bc65-545379793b91.png)

🚩In our Shipping Analysis page, we prepared a variety of visualizations that will be used conjunctly with our geo map in analysis. The first chart is a bar graph of sales revenue per region. This chart is linked to our geo map and will filter regions on the geo map based on chart selection. 

![9-12](https://user-images.githubusercontent.com/92877810/139945769-1072aa8a-9e75-418c-b099-bd07f57944a3.png)

🚩The second visualization is a table displaying the No of Delivered Orders and Avg Delivery Times for stores in our shipping model. This chart has linked analysis filtering applied from our geo map and will filter entries based on selections made on our geo map. 

![9-13](https://user-images.githubusercontent.com/92877810/139945772-c171ff2a-6829-4a32-986a-f1048b791a0c.png)

11. Scroll to the bottom 

12. Select the Geo Map already created for you

![9-14](https://user-images.githubusercontent.com/92877810/139945773-cec40f1d-ef04-40ce-b0df-b3d63f23ea68.png)

13. Click **Designer** to open Builder Panel (in case not already open) 

🚩We want to choose a layer that will help us visualize the distribution of our measure, Average Delivery Time, in our geo visualization. The Heat Map Layer is a good way to visualize the data density of a measure on our map. Let us create this layer in our geo map 

14. Click **Add Layer**

![9-15](https://user-images.githubusercontent.com/92877810/139945777-b323ee27-0527-497b-bfa6-e8207a031d90.png)

15. Rename the layer to **Order Delivery Time Density**

Let us change the model for this layer to the shipping model which contains our desired measures. You can add layers sourcing measures and dimensions from multiple models on a single geo visualization, enhancing your ability to compare data. 

16. Click **Select Model**

![9-16](https://user-images.githubusercontent.com/92877810/139945779-cf580dd3-555b-46b4-93fa-cb95d6744a2d.png)

17. Click **ANA260_SHIPPING_INFO**

![9-17](https://user-images.githubusercontent.com/92877810/139945780-e14aa69c-9798-4170-97a1-e84f1f646268.png)

18. Click **OK**

![9-18](https://user-images.githubusercontent.com/92877810/139945781-710a5636-98de-41ea-b2dc-c412b8d41ef3.png)

ℹ️SAP Analytics Cloud offers a variety of layers for geographical visualizations. The most common used ones are  
Bubble Layer, which shows each location as a bubble. Using color and size of the bubble allows us to see correlation between different measures 
Choropleth Layer shows the shape of a geo location and allows drilling from aggregated levels such as country into smaller areas such as regions 
Heat Map Layer, allows to show the concentration of geographical locations 
 
For your next step you would like to view your data in a heat map.

19. Click **Choose Layer Type**

20. Click **Heat Map Layer**

![9-19](https://user-images.githubusercontent.com/92877810/139945783-e2be03c5-a1a7-4cb0-9c53-499a843f2b5e.png)

ℹ️Let us add our geo enriched dimension to this geo map.

21. Click **+ Add Location Dimension**  

![9-20](https://user-images.githubusercontent.com/92877810/139945785-9770e920-3c46-44f4-b3fb-9eaed7cc1f65.png)

22. Click **Store Location**

![9-21](https://user-images.githubusercontent.com/92877810/139945787-59127c41-ed60-4249-9694-c494c5d6dcea.png)

🚩We want to look at Avg Delivery Time, a calculated measure in our model, to look at the density of delivery times in our heat map layer. 

23. Click **Add Measure**

![9-22](https://user-images.githubusercontent.com/92877810/139945789-4bb675cc-73d7-4c1c-a88d-567a15e1080f.png)

24. Scroll and click **Avg Delivery Time** 

![9-23](https://user-images.githubusercontent.com/92877810/139945791-68c6428e-7eab-4896-bcec-a9cbd34009fe.png)

25. Click **OK**

![9-24](https://user-images.githubusercontent.com/92877810/139945793-ad420e72-efb1-47a6-8f16-e804336cbe06.png)

⚠️Quality check! Does your geo map look like this screenshot after applying the heat map layer and zooming in? 

🚩Our Heat Map layer looks great, but the scale may be too large for our desired purpose. We can change the gradient properties of our heatmap to improve our visualization and make it easier to discover clusters of outlier delivery times. 

![9-25](https://user-images.githubusercontent.com/92877810/139945795-53f5e579-fed1-4983-b245-193eff29ebf8.png)

26. Click **Edit Layer**

![9-26](https://user-images.githubusercontent.com/92877810/139946257-dcba97a3-3586-4355-b5b7-b33e9acdba48.png)

🚩Let us reduce the blur radius so it is clearerwhere our high and low average delivery times are present in Spain. The blur radius determines the size of each data point and how it overlaps with other values. We can improve the definition between pointsby reducing the blur radius. 

27. Click **Expand** on **Avg Delivery Time**

28. Change the Blue Radius from 40% to 20% 

29. Click **OK**

![9-27](https://user-images.githubusercontent.com/92877810/139946258-1fd6cd83-a65d-4c84-adbc-37347905d5b6.png)

⚠️Quality check! Does your geo map look like this screenshot after changing the blur radius? 

![9-28](https://user-images.githubusercontent.com/92877810/139946259-3ecc8b6b-0bbf-4500-b916-b58f4463dca6.png)

🚩Let us move our geo map back to look at delivery times in **Spain** 

30. Click into our Geo Map, hold and drag to be looking at **Spain** 

31. Zoom into the cluster in Spain by scrolling your **mouse wheel up**. 

![9-29](https://user-images.githubusercontent.com/92877810/139946261-2cd51f97-9c8d-4565-9743-ec66d9dc5058.png)

🚩You can change the appearance of the heat map layer as well by zooming in and out of the geo map and focusing on areas of interest. When we zoom into Spain, we notice there are some distinct clusters of higher average delivery times. Let us investigate this further. 

![9-30](https://user-images.githubusercontent.com/92877810/139946262-aef5af9d-63c1-4687-a8bb-b4bd551d5443.png)

🚩Let us create a new layer that looks at our delivery time measures at a store level. First, let us hide our heat map layer. 

32. Click **Hide** on **Order Delivery Time Density**

33. Click **+ Add Layer**

![9-31](https://user-images.githubusercontent.com/92877810/139946264-48257015-bba6-43eb-8e8d-8e6e4c762ae6.png)

🚩We are going to create a layer that shows our delivery measures on a store by store basis to further our analysis 

34. Rename the layer to **Store Location Analysis**

35. Select **ANA260_SHIPPING_INFO** if not already selected 

![9-32](https://user-images.githubusercontent.com/92877810/139946265-8b575a32-844f-4935-9a85-e991e7af7ed5.png)

🚩We want the ability to drill up and down in our layer from a store level to an aggregated country level (i.e.Spain). Let us choose to create a choropleth layer. 

36. Click **Choose Layer Type**

37. Click **Chloropleth/ Drill Layer**

![9-33](https://user-images.githubusercontent.com/92877810/139946266-cb2e2d04-bdd3-466f-993a-63796505eb01.png)

🚩We can choose to use bubble instead of choropleth in the style of our drill down layer. This will represent our hierarchy members in the form of bubbles on the geo map. Since we want to look at individual stores, this is preferred! 

38. Click **Choose Style**

39. Click **Bubble**

![9-34](https://user-images.githubusercontent.com/92877810/139946269-42b77103-6912-4948-8bc6-45d1fe10dabe.png)

40. Click **+ Add Location Dimension**

![9-35](https://user-images.githubusercontent.com/92877810/139946270-389fab5a-a395-4e41-a4ea-1e9291896569.png)

41. Click **StoreLocation**

![9-36](https://user-images.githubusercontent.com/92877810/139946848-6eefaec3-c52d-45db-9618-c20e396de9f7.png)

42. Click **Add Measure/Dimension**

![9-37](https://user-images.githubusercontent.com/92877810/139946850-34f28743-3978-46a3-a5d5-197ad6d1bd7a.png)

🚩Let us add additional measures into our analysis. We can choose to color code our bubbles with the **Average # of Delivered Orders** to see if this measure is related to our delivery times. 

43. Click **Average # of Delivered Orders**

![9-38](https://user-images.githubusercontent.com/92877810/139946852-36b90b49-16a0-4a3e-b095-0f76890807e8.png)

44. Click **+ Add Measure**

![9-39](https://user-images.githubusercontent.com/92877810/139946853-373334af-b184-4911-b298-286158412082.png)

🚩We are choosing average delivery time as our bubble size, so it is easy to pinpoint which stores are outliers in our modeled data. 

45. Scroll and Click **Avg Delivery Time**

![9-40](https://user-images.githubusercontent.com/92877810/139946856-867afdb0-045e-4bc0-bd32-21cff62643b5.png)

⚠️Quality check! Does your geo map look like this screenshot after adding the new choropleth layer? 

![9-41](https://user-images.githubusercontent.com/92877810/139946857-d0b1feae-d992-4488-9c44-e592150a4a6d.png)

🚩Based on our current geo map, the sizing of our bubbles does not suit our analysis of delivery times. We can customize how our measure is translated into bubble size to improve our visualization 

46. Click **Expand on Avg Delivery Time**

🚩Changing the range for our bubbles will help us identify outliers in our geo map based on our measure, Avg Delivery Time. Let us changes these ranges for the hierarchy levels we are interested in: Country, Region, and StoreLocation. 

47. Expand **Range** for **Country**

48. Change upper range from **100%** to **500**

49. Click outside the pop-up. 

![9-42](https://user-images.githubusercontent.com/92877810/139946859-a0959dc9-c640-4f27-801d-2d863ce6fb0b.png)

50. Expand **Range** for **Region**

51. Change upper range from **100%** to **500%**

52. Click outside the pop-up. 

![9-43](https://user-images.githubusercontent.com/92877810/139946860-2f955a3e-de7e-4d21-9951-45bbedcb6a80.png)

53. Expand **Range** for **StoreLocation**

54. Change upper range from **100%** to **500%**

55. Click outside the pop-up. 

56. Click **OK**

![9-44](https://user-images.githubusercontent.com/92877810/139946861-141f24a5-6da6-4040-8a3c-1eef5fdd7d92.png)

⚠️Quality check! Does our geo map look like this screenshot after Bubble Size changes? It is now much easier to differentiate the hierarchy level members on our geo map. 
 
![9-45](https://user-images.githubusercontent.com/92877810/139946862-34e016bd-7fec-430b-bea2-442e677bb619.png)

57. Click **Spain**

58. Click **Drill Down**

![9-46](https://user-images.githubusercontent.com/92877810/139946864-963388e4-26cb-4139-a565-2e6e4e4d4088.png)

⚠️Quality check! Does your geo map look like this screenshot after drilling down? 

🚩We can see that the La Rioja region in Spain seems to have high average delivery times (with its large bubble) and high numbers of delivered orders. On the other hand, Castilla Leon has very low average delivery times. This is very informative, and we should look at this layer on an individual store level. 

![9-47](https://user-images.githubusercontent.com/92877810/139946866-ba2df4a4-8bbb-431f-8258-6b4dfd5bc753.png)

🚩Before we drill down again, let us check to see how our hierarchy is defined. 

59. Click **Navigate up/down the hierarchy**

🚩Let us choose the hierarchy for the current map layer we are looking at. 

60. Click **Store Location**

![9-48](https://user-images.githubusercontent.com/92877810/139946867-1a690568-778f-4912-9a29-3e3ca8cd146d.png)

🚩As we can see, there are 2 additional hierarchy layers, Sub-Region 1 and Sub-Region 2, before we reach our desired StoreLocation level. Let us simplify our hierarchy to two levels, Country and StoreLocation, for efficiency purposes 

![9-49](https://user-images.githubusercontent.com/92877810/139946868-ca9bf2ba-1420-44b2-b518-e351a4caca6a.png)

🚩We can customize which hierarchy levels are drillable in our choropleth layer. This is a performance best practice tip! Rendering additional hierarchy levels that we are not interested in is both time and resource intensive. 

61. Click the **Hierarchy** option for **Store Location Analysis**

![9-50](https://user-images.githubusercontent.com/92877810/139946873-3d1fbe63-9162-4f86-8a9e-240ab56f539d.png)

62. Uncheck **Show Region**

63. Uncheck **Show Sub-Region 1**

64. Uncheck **Show Sub-Region 2**

65. Click **Save**

![9-51](https://user-images.githubusercontent.com/92877810/139946874-1f1fc7b7-39ba-4dd3-addf-b9f184681d61.png)

⚠️Quality check! Does your geo map look like this screenshot? Now, that we have changed the hierarchies, our geo map has reset to the country hierarchy level as the primary level. 

![9-52](https://user-images.githubusercontent.com/92877810/139946875-1fbe0ccc-3799-4aac-b8a1-ed261dd46587.png)

🚩Let us try drilling into Spain and see if we reach our desired hierarchy level. 

66. Click on **Spain**

67. Click **Drill Down**

![9-53](https://user-images.githubusercontent.com/92877810/139946880-5589a9d0-68a6-4dbc-abca-847966b9d76d.png)

⚠️Quality check! Does your geo map look like this screenshot after drilling down on Spain? 

![9-54](https://user-images.githubusercontent.com/92877810/139946881-12c29fe9-214d-43f0-99f2-ac290ced67de.png)

🚩Let us double check to see if our geo map only displays these two hierarchy levels 

68. Click Navigate up/down the hierarchy  

69. Click StoreLocation 

![9-55](https://user-images.githubusercontent.com/92877810/139946884-5502bb7c-8bf8-4443-8282-586664c60ddb.png)

🚩As we can see our hierarchy levels for this layer are properly defined. Let us look at the insights on our StoreLocation hierarchy. Definite Gains Gym seems to be an outlier in high delivery times from the La Rioja region and trainingapparel4sale.com is an outlier in low delivery times from the Castilla Leon region. 

![9-56](https://user-images.githubusercontent.com/92877810/139946885-db6cbe9a-4c91-486c-9f1d-32e86afb90d8.png)

70. Right Click on the Geo Map to open **Context Menu**

![9-57](https://user-images.githubusercontent.com/92877810/139946886-25b14930-25c7-4783-b4f8-5364b082ac7f.png)

71. Click **Show/Hide**

72. Hover over **Store Location Analysis**

73. Click **Average Delivery Time (Size)**

74. Click outside to collapse the context menu 

![9-58](https://user-images.githubusercontent.com/92877810/139946888-e5ab5775-dba5-423b-8a12-224e3fca5f5b.png)

⚠️Quality check! Does your geo map look like this screenshot? We can see from the labels that both stores, Definite Gains Gym and trainingapparel4sale.com, have outlier average delivery times. 

![9-59](https://user-images.githubusercontent.com/92877810/139946890-e1793342-916e-486f-9864-eb9cda1d9f51.png)

ℹ️We can also display measure values in interactions with the geo map. 

75. Click **Edit Layer** for **Store Location Analysis**

![9-60](https://user-images.githubusercontent.com/92877810/139946891-0b4e2a13-abdb-4148-9b56-fea433becff7.png)

🚩Let us add a tooltip for our Average # of Delivered Orders measure. 

76. Click **Add Tooltip**

77. Click **Tooltip Information** 

![9-61](https://user-images.githubusercontent.com/92877810/139946892-8a1925f9-4ec4-4e87-9f2a-916f145c2410.png)

78. Click **+ Add Measures/Dimensions** under Tooltip Information 

![9-62](https://user-images.githubusercontent.com/92877810/139946893-db8e2046-a3b4-4be4-a833-346287158ebc.png)

79. Click **Average # of Delivered Orders**

![9-63](https://user-images.githubusercontent.com/92877810/139946894-a5081195-8ee6-4a9c-aa1b-a4a67edb86de.png)

80. Click **OK**

![9-64](https://user-images.githubusercontent.com/92877810/139946895-a64aef42-18f4-4aad-a020-f550fcbbb0a0.png)

⚠️Quality Check! Does your geo map look like this screenshot? 

![9-65](https://user-images.githubusercontent.com/92877810/139946898-addf1ffa-7625-4612-9d68-0f6bde3236b1.png)

Let us see what the tooltip looks like when we hover over a bubble. 

81. Hover over **Definite Gains Gym**

![9-66](https://user-images.githubusercontent.com/92877810/139946900-443acaf7-ac5e-463f-9d15-52f919afe98c.png)

🚩We want to add a new layer for analysis which will require some data preparation 

ℹ️In this next part of the Geo Visualization deep dive we will look at how to create a geo-enriched model. We want to add a geo-enriched model for Shipping Port locations that will be used as the next layer in our geo map analysis. 

**Please save your story by pressing Ctrl + S on your keyboard.**

![9-67](https://user-images.githubusercontent.com/92877810/139946904-69663a4d-fd98-4157-94b5-b0579a87c536.png)

82. Click **Menu**

![9-r](https://user-images.githubusercontent.com/92877810/141177930-e08c8d53-d9ac-4097-93cc-c6315ae41474.png)

83. Click **Modeler** to create a new model 

![9-r2](https://user-images.githubusercontent.com/92877810/141177932-6c15bbf1-222f-4cb4-b0eb-21bddc671aa0.png)

🚩We want to start our model based on the Shipping Ports Excel file, which is located in GitHub. 

To access the Shipping Ports file, please navigate to our ANA260 GitHubrepository. You can access this at https://github.com/SAP-samples/teched2021-ANA260 

84. Click on the **exercises** folder 

![9-69](https://user-images.githubusercontent.com/92877810/139946907-577fa954-e34b-4b4b-8f1e-91b1e8f60282.png)

85. Open the **Resources** folder 

![9-70](https://user-images.githubusercontent.com/92877810/139946908-6ddb6b4f-52f1-4051-8811-4104d6664384.png)

86. Click **Shipping Ports.xlsx**

![9-71](https://user-images.githubusercontent.com/92877810/139946909-d47e72f3-9f29-4946-be95-191cefd15a9a.png)

🚩Please download the Excel file onto your computer so you can import it into SAP Analytics Cloud as an acquired model.

87. Click **Download**

![9-72](https://user-images.githubusercontent.com/92877810/139954383-38f972ef-03a0-444b-9d51-1247a3009cdd.png)

🚩  
Navigate back to SAP Analytics Cloud

88. Click Import **From a CSV or Excel File**

![9-73](https://user-images.githubusercontent.com/92877810/139954385-17281bf8-cec2-4944-9ebb-7eb791b7c8bd.png)

89. Click **Select Source File**

![9-74](https://user-images.githubusercontent.com/92877810/139954386-0255d774-0fe0-41ce-81d2-29e7bd44721f.png)

ℹ️Once the Shipping Ports.xlsx is downloaded, open the Downloads folder on your machineto select the file.

90. Select the **Shipping Ports.xlsx** file

91. Click **Open**

![9-75](https://user-images.githubusercontent.com/92877810/139954387-e6a5dc61-d8e9-4a38-8d18-6feb0c92a7b3.png)

92. Click **Import**

![9-76](https://user-images.githubusercontent.com/92877810/139954389-49a49fd4-1857-4201-b2dc-2b9cdf5e54a8.png)

⚠️Quality Check! Does your imported file bring you to a model creation screen like this screenshot

🚩Welcome to Data Modeling in SAP Analytics Cloud!
 
In this screen, users can assign dimensions and measures, build hierarchies in their data, apply transformations on columns of data, check for and replace wrong data entries, and geo enrich their data. If you are importing a large data set, this screen will show a subset of your data, so it is easier to work with. SAP Analytics Cloud will apply all your requested changes to your entire data set when creating the model.

![9-77](https://user-images.githubusercontent.com/92877810/139954390-0258271f-fb93-4568-b5ba-654728b63ab4.png)

🚩Let us geo enrich our model so it can be used in our geo visualization. Model creators can choose to geo enrich their data by coordinates (latitude and longitude) or by location name (country and region name). Country data can be imported by ISO3 and ISO2 codes or by Englishnames.

93. Click **Geo Enrichment**

94. Click **Coordinates**

![9-78](https://user-images.githubusercontent.com/92877810/139954391-8630d971-9e77-4ac1-9afc-0f2c20993c16.png)

🚩Let us choose an Identifier for our geo enriched Location dimension. This will be thelabel used for each node in a geo map layer. Let us use the Shipping Port names as the description.

95. Click **Location Description**

96. Click **Port**

![9-79](https://user-images.githubusercontent.com/92877810/139954392-ceea855e-07f7-4dd1-a262-ef4f39d52caa.png)

97. Click **Create**

![9-80](https://user-images.githubusercontent.com/92877810/139954393-bc8fb881-e685-4bb0-9c40-c4366e3c372d.png)

⚠️Quality check! Does your model creation screen have a new dimension like this Location column in the screenshot?

![9-81](https://user-images.githubusercontent.com/92877810/139954395-0a282ed9-abf6-4eb8-9d0e-787c8ea29344.png)
  
🚩Let us now create our model with the geo enriched dimension. You may notice that there area few invalid data points in our geo enriched dimension due to incorrect longitude and latitude data. SAP Analytics Cloud warns model creators about potential errors in the data. The model can still be created and the rows containing faulty data will be excluded from the model. You can choose to replace these invalid data cells directly in the model creation screen.

98. Click **Create Model**

![9-82](https://user-images.githubusercontent.com/92877810/139954397-ee0a1aab-a02a-4c9e-8145-93dad45381bb.png)

99. Click **Create**

![9-83](https://user-images.githubusercontent.com/92877810/139954398-c8ee441a-e9ed-479b-93c9-1b77e2278b81.png)
  
🚩Let us name our model **ShippingPorts** and save it in our MyFiles directory on the tenant.

100. Click **OK**

![9-84](https://user-images.githubusercontent.com/92877810/139954399-5e64e171-b661-4b26-8d8c-acc2bf3ffc82.png)

⚠️Quality check! Your screen should now display this Model creation in prompt.

![9-85](https://user-images.githubusercontent.com/92877810/139954400-76224d5c-895d-4a4b-9a1e-07cb3ac1a786.png)
  
⚠️Quality check! Our model creation is successfully complete! Do you see a screen like this screenshot?
 
Note that some of the rows were rejected due to incorrect locations.
  
ℹ️After this stage, we can navigate back to our **"ANA260_Section 9_Your Initials"** story and continue our analysis with our new ShippingPorts model!

![9-86](https://user-images.githubusercontent.com/92877810/139954403-cfa5e7c2-23a0-4206-82cd-99297edcd64d.png)

101. Click **Home**

![9-87](https://user-images.githubusercontent.com/92877810/139954405-99eeceb2-0842-426a-9dbf-be98dbefa841.png)

ℹ️Since we just used the Geo story before, we can open it via the recently used stories tiles on the homepage.

102. Select the last story you worked on (ANA260_Section 9_Your Initials)

![9-88](https://user-images.githubusercontent.com/92877810/139954407-cc99cdc0-2053-4d90-85f6-b9013f1512f9.png)

103. Click **Edit**

![9-89](https://user-images.githubusercontent.com/92877810/139954408-7300f45c-85bb-4a0d-929a-4ac972c735b3.png)

104. Click **Shipping Analysis**

![9-90](https://user-images.githubusercontent.com/92877810/139954409-82a3f1e3-6af5-4487-b472-c4d3e66b16d8.png)

105. Select the **Geo Map**

106. Click **Designer**

![9-91](https://user-images.githubusercontent.com/92877810/139954410-1224b5a4-8598-44f4-8995-40d4d362196b.png)

🚩Let us add a new layer with our new geo enriched model.

107. Click **+ Add Layer**

![9-92](https://user-images.githubusercontent.com/92877810/139954413-b246e806-0ffc-4ff0-9a08-27c5eff8ea06.png)

108. Rename Layer to **Shipping Port Location**

109. Click **Change Model**

![9-93](https://user-images.githubusercontent.com/92877810/139954414-bc9ee6ba-86e7-486b-824e-71083342b73f.png)
  
🚩Since our model is new to this story, we will have to select it from our files first.

110. Click **Select other model...**

![9-94](https://user-images.githubusercontent.com/92877810/139954416-44fb2e19-f307-4d39-ab9c-6bd25fa481f2.png)

🚩Navigate to where you saved the ShippingPorts model (My Files directory).

111. Click **ShippingPorts**

![9-95](https://user-images.githubusercontent.com/92877810/139954418-205ace14-8174-4de3-9e2e-3fcc3810d885.png)

ℹ️Let us add the geo enriched dimension we created with coordinates

112. Click **+ Add Location Dimension**

![9-96](https://user-images.githubusercontent.com/92877810/139954421-22004dc1-08b3-4e7c-9323-31b404926c87.png)

113. Click **Location**

![9-97](https://user-images.githubusercontent.com/92877810/139954422-6ec74605-ddb9-454c-8357-25077baac0f4.png)

⚠️Quality check! Does your geo map now populate with shipping port bubbles like this screenshot?

![9-98](https://user-images.githubusercontent.com/92877810/139954424-ee8c5793-5c3e-4887-9e02-a9a674d5fc71.png)

🚩Let us change the shape of our shipping port bubbles so they are easily distinguished fromour stores.

114. Click **Expand**

115. Click **Shapes**

116. Choose the **Star** shape

117. Click **OK**

![9-99](https://user-images.githubusercontent.com/92877810/139954425-45e7c89f-17bf-4b40-ad8e-275e4059f12e.png)

⚠️Quality check! Does your geo map look like this screenshot with the shipping port shape changes?

![9-100](https://user-images.githubusercontent.com/92877810/139954429-529a8f27-283e-4dee-b7e5-a14e88865566.png)
  
🚩We can now choose to add a filter between our two location dimensions, Store Location and Shipping Port Location, to generate additional analysis in our geo visualization

118. Click **+ Add Filter**

![9-101](https://user-images.githubusercontent.com/92877810/139954430-f9cf4ef3-17eb-4544-ad1f-8d9e218847dd.png)

ℹ️We want to test a hypothesis if distance to shipping ports affect delivery times. We will create a distance filter based on the distance from a shipping port. If a store is further from a shipping port than our defined distance, it will be excluded from our geo map.

![9-102](https://user-images.githubusercontent.com/92877810/139954431-fd79aecb-79f6-4306-a1b1-a0c69282408a.png)

🚩Our Show parameter is the dimension that we would like to exclude members based on our distance filter.

119. **Expand** Show Dimension

120. Click **StoreLocation** as the Show Dimension

![9-103](https://user-images.githubusercontent.com/92877810/139954432-45eb583c-4004-434a-8024-95091b2fde18.png)

🚩Let us add an interactive input control slider to our page to dynamically change the distance in distance filter.

121. Check **Add as an input control slider to page**

122. Input **1** as Minimum Distance 

123. Input **6000** as Maximum Distance 

![9-104](https://user-images.githubusercontent.com/92877810/139954433-207e58da-5e25-4fb2-9a7a-5f52bf280ded.png)

🚩Let us choose the Shipping Port locations as our reference location to measure the distance from.

124. Click **Select a Reference Location**

125. Click **Dimensions**

![9-105](https://user-images.githubusercontent.com/92877810/139954436-1814dc16-f163-4207-95de-aa20e2975604.png)

126. Choose **Location** dimension from ShippingPorts model.

![9-106](https://user-images.githubusercontent.com/92877810/139954437-ed3d141c-6e15-4bca-a0bd-011da8e16e4e.png)

127. Click **OK**

![9-107](https://user-images.githubusercontent.com/92877810/139954439-b9460787-06c3-4230-8c4e-f383b1e773b6.png)

⚠️Quality check! Does your geo map look like this screenshot? Since our distance filter has defaulted to 1km, there should be no stores displayed on our geo map as they areall excluded currently.

![9-108](https://user-images.githubusercontent.com/92877810/139954441-a15b455b-c641-47c9-b713-323984d8bb5a.png)

🚩Let us resize our input control so it is easier to read and dynamically change.

128. Expand the Input Control by dragging on the bottom right corner

![9-109](https://user-images.githubusercontent.com/92877810/139954444-f3f0b05b-330f-4884-a184-5bb539db827c.png)

⚠️Quality check! Does your distance filter input control look like this after resizing?

![9-110](https://user-images.githubusercontent.com/92877810/139954445-fd9dcc8c-5cfb-4332-81d3-cf3a1eb32fef.png)

🚩Let us start with a medium distance filter.

129. Change the distance filter to 275

![9-111](https://user-images.githubusercontent.com/92877810/139954446-ad13e8b6-fb20-4601-b912-db49563d7f7f.png)

⚠️Quality check! Does your geo map look like this screenshot? Interestingly, our high average delivery time outlier, Definite Gains Gym, shows up but our other low average delivery time outlier, trainingapparel4sale.com, is missing.

![9-112](https://user-images.githubusercontent.com/92877810/139954448-68dbd4ac-c7c0-424a-8260-8c64396ff73b.png)

🚩Let us increase the range of our distance filter.

130. Change the distance filter to 500

![9-113](https://user-images.githubusercontent.com/92877810/139954449-f9be75b7-3365-4172-9e39-86f42c5b96b2.png)

⚠️Quality check! Does your geo map look like this screenshot?Now most of our stores in Spain have appeared from the filter.

![9-114](https://user-images.githubusercontent.com/92877810/139954451-845aa052-7bd1-47c7-959c-5b5a4ac3ea1a.png)

🚩Let's add **Linked Analysis** on our Geo Map

131. Click **More** icon

132. Click **Linked Analysis**

![9-115](https://user-images.githubusercontent.com/92877810/139954453-43fa301d-3210-474b-b499-010dc7c714e5.png)

133. Click **Only Selected Widgets**

![9-116](https://user-images.githubusercontent.com/92877810/139954454-21afc2f0-d65a-4462-a149-d344d47dc14d.png)

134. Select **Filter on Data Point Selection**

![9-117](https://user-images.githubusercontent.com/92877810/139954455-cb135b81-54a9-47fd-8c3e-be113d4a649c.png)

135. Scroll and Select **Store Region wise Delivery Time and # of Delivered Orders..**

136. Click **Apply**

![9-118](https://user-images.githubusercontent.com/92877810/139954457-8b3c73b5-d3ce-46d3-b9a1-8871532c2864.png)

ℹ️Let us filter directly on our two outlier stores for Avg Delivery Time.

137. Mouse wheel up in the geo map to zoom in on Spain

![9-119](https://user-images.githubusercontent.com/92877810/139954458-ea643b8a-5c08-4635-85ab-898fefe4bf5f.png)

ℹ️We want the ability to be able to select many data points on our geo map directly and easily filter on a selected area. Let us use the lasso functionality in geo maps.

138. Click the **Lasso Tool**

![9-120](https://user-images.githubusercontent.com/92877810/139954461-c5730895-ba7c-4545-9d7f-70e0d62fc932.png)

139. Draw a lasso around **Definite Gains Gym and trainingapparel4sale.com**

![9-121](https://user-images.githubusercontent.com/92877810/139954463-8e94a982-6a3a-4e89-bb70-a2fd2c0ae527.png)

🚩We can now choose to apply a filter on the bubbles selected by our lasso tool.

140. Click the **Filter Icon**

![9-122](https://user-images.githubusercontent.com/92877810/139954465-2f71a45e-d50b-4f41-90a7-d7bafbea8e76.png)

⚠️Quality check! Does your geo map look like this screenshot after filtering on lasso tool?

![9-123](https://user-images.githubusercontent.com/92877810/139954467-b01e26de-af2d-4389-8a15-4ecd49195d97.png)

🚩We can also look at our table that is connected to our geo map by linked analysis applied on data point selection. We can see the measures in this table for our two filtered entries.

![9-124](https://user-images.githubusercontent.com/92877810/139954470-d593c256-c996-48da-9720-095c267d8815.png)

🚩Since we did not verify our hypothesis that distance to shipping ports is the cause for a higher average delivery time, let us dive into another tool we can use for analysis in our geo map.

141. Select our Geo Map and click on **Designer**

![9-125](https://user-images.githubusercontent.com/92877810/139954472-fc034328-ea01-4a9b-8472-1c958ea74239.png)

ℹ️We can change the basemap layer in our visualization to better fit the purposes of our analysis. Let us see if there is a geographical reason forthe outliers in delivery time. For now, we want to see if there are any insights that we can gather from the street map view in our geo map

142. Click **Choose Basemap**

143. Click **OpenStreetMap**

![9-126](https://user-images.githubusercontent.com/92877810/139954473-ca99f466-4e59-4b62-b91d-5116c8423c34.png)

⚠️Quality check! Does your geo map look like this screenshot after changing the base map? Let us change the formatting to make analyzing this visualization easier

![9-127](https://user-images.githubusercontent.com/92877810/139954478-fea7db17-776d-4109-831c-67d0a5ca1aff.png)

🚩First, let us change the font color so it stands out on our base map.

144. Click **Styling Panel**

![9-128](https://user-images.githubusercontent.com/92877810/139954483-daa9a143-8821-4fba-a991-05411e356c9e.png)

ℹ️We can change formatting options for all text in the geo map or based on individual layers. We want to select the Store layer to change the color on Store name labels.

145. Scroll to Font Options and click **Text Selection**

146. Click **Store Location Analysis**

![9-129](https://user-images.githubusercontent.com/92877810/139954484-b3e9215a-db3b-4653-bfa9-1dbc2dbacc8d.png)

147. Click **Color**

148. Select **Black Palette**

![9-130](https://user-images.githubusercontent.com/92877810/139954485-600e6041-9332-408f-b3ef-726c2117dc72.png)

🚩Let us now change the Basemap properties to complement our styling change

149. Click **Builder Panel**

![9-131](https://user-images.githubusercontent.com/92877810/139954486-5c60bed6-990c-401d-adf9-b79ff1604043.png)

🚩We can change the Basemap Opacity,so our layers stand out in our geo map

150. Click **Expand**

151. Change Basemap Opacity from **100%** to **50%**

![9-132](https://user-images.githubusercontent.com/92877810/139954487-e7e03dc2-0942-4575-b3e4-3cd3c5154c58.png)

⚠️Quality check! Does your geo map look like this screenshot after applying styling changes?

🚩If we lookat the geo map, a new hypothesis for delivery times can be formed. trainingapparel4sale.comis located directly on a major highway connected to Madrid whereas Definite Gains Gym is secluded and much further from major transit routes. This potentially explains our outliers for average delivery times.

![9-133](https://user-images.githubusercontent.com/92877810/139954488-18c2f7f5-fbda-4669-9e13-80ef30c6dfe5.png)

🚩Let us move forward and change our Basemap back to a standard template to try out other geo visualization features.

152. Click **Choose Basemap**

153. Click **Light Gray**

![9-134](https://user-images.githubusercontent.com/92877810/139954491-dae5c11c-a6e2-4674-a03b-0099568c3afd.png)

⚠️Quality check! Does your geo map look like this screenshot after basemap changes?

![9-135](https://user-images.githubusercontent.com/92877810/139954494-f0b24b7a-0284-42ab-85b1-b53a17dcf4e8.png)

🚩We want to look at a different area in the geo map. Let us move backto general view by removing all our applied filters.

154. Click **Remove Filters**

![9-136](https://user-images.githubusercontent.com/92877810/139954496-e19206fd-d0e7-42fc-a833-dcc588acd06f.png)

🚩Let us also drill up to the country hierarchy level.

155. Click on a Store Bubble

156. Click **Drill Up**

![9-137](https://user-images.githubusercontent.com/92877810/139954499-da5e2afb-9089-417d-b6d3-ace47518d93c.png)

⚠️Quality check! Does your geo map look like this screenshot?

![9-138](https://user-images.githubusercontent.com/92877810/139954501-4f803ecd-99f6-4422-9005-5a0d6bf175be.png)

🚩We can also choose to change our layer options in the Legends tab of the geo map. This enables us to change our geo map display in View Mode without accessing the Designer Panel.

157. Click **Expand Legends**

![9-139](https://user-images.githubusercontent.com/92877810/139954503-77e0fff1-28b0-49ae-9354-e56a5bb91556.png)

🚩Let us show the original choropleth layer for sales revenue and hide the other layers we have created. We want to go back to our chart analysis of sales revenue across all regions in our geo map.

158. Click **Hide Layer** for Shipping Port Layer.

159. Click to **Collapse Legends**

![9-140](https://user-images.githubusercontent.com/92877810/139954506-66bbb938-9b17-4ef7-a9b4-58386116d59a.png)

⚠️Quality check! Does your geo map look like this visualization?
  
🚩Please save your story by pressing Ctrl + S on your keyboard!

![9-141](https://user-images.githubusercontent.com/92877810/139954509-31016ab8-3187-445e-8824-6c3bc49e7e83.png)

ℹ️You have now completed the **Geo Visualizations** Deep Dive section!
![9-142](https://user-images.githubusercontent.com/92877810/139954511-fa6c3750-14fa-42b1-9bd2-472255410dd3.png)

<br><br>

## Summary

**You have completed the entire Geo Visualizations section!**

**You are now able to:**
- Create your own geo-enriched models with acquired data
- Employ heat maps to gather insights on geo data density
- Understand the use of distance filters and the lasso tool in analyzing your hypotheses
- Use tooltips, labels, and overlapping points to enhance the insights in your geo map
- Change your basemap layer to view your geo enriched data in different contexts
- Style your geo map for clear and informative visualizations

