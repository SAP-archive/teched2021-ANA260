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

27. Click **Expand on Avg Delivery Time**

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

48. Change upper range from **100%** to **500% **

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

82. Click **More** to open the menu 

83. Click **Modeler** to create a new model 

![9-68](https://user-images.githubusercontent.com/92877810/139946906-aa50ecd8-f4df-4afd-8a6c-31905caa8245.png)

🚩We want to start our model based on the Shipping Ports Excel file, which is located in GitHub. 

To access the Shipping Ports file, please navigate to our ANA260 GitHubrepository. You can access this at https://github.com/SAP-samples/teched2021-ANA260 

84. Click on the **exercises** folder 

![9-69](https://user-images.githubusercontent.com/92877810/139946907-577fa954-e34b-4b4b-8f1e-91b1e8f60282.png)

85. Open the **Resources** folder 

![9-70](https://user-images.githubusercontent.com/92877810/139946908-6ddb6b4f-52f1-4051-8811-4104d6664384.png)

86. Click **Shipping Ports.xlsx**

![9-71](https://user-images.githubusercontent.com/92877810/139946909-d47e72f3-9f29-4946-be95-191cefd15a9a.png)

