
⚠️**Excercise Check!** Does your story look like this? 

![9-1](https://user-images.githubusercontent.com/92877810/139740637-c40c7f10-e4d1-4ea2-8aed-633989fd8aa0.png)

1. Click **Files**

![9-2](https://user-images.githubusercontent.com/92877810/139740639-fd6dea9e-94a2-4ea0-b9b6-7f01334b770c.png)

👉If you are not in the TechEd 2021 folder, follow the path: **Public/TechEd 2021**

2. Select **Section 9.0 - Geo Visualizations(Start)**

3. Click **Copy To**

![9-3](https://user-images.githubusercontent.com/92877810/139740640-a7364740-d27f-4d6e-9d06-7fceb0060743.png)

4. Click **MyFiles**

![9-4](https://user-images.githubusercontent.com/92877810/139740641-e4996336-a389-41d1-9d56-c23052cbc658.png)

5. Save the file in MyFiles under the name **"ANA260_Section 9_Your Initials"**

6. Click **OK**

![9-5](https://user-images.githubusercontent.com/92877810/139740643-ad896924-cef9-4246-9d3f-2ab315da6d1a.png)

7. Click **MyFiles**

![9-6](https://user-images.githubusercontent.com/92877810/139740645-d4f0fe28-780e-4bf0-8e68-7efb65e113ea.png)

8. Open **ANA260_Section 9_Your Initials** file

![9-7](https://user-images.githubusercontent.com/92877810/139740646-e8a2ec27-8d6a-419b-91eb-d0fa5cd7ff19.png)

9. Click **Edit**

![9-8](https://user-images.githubusercontent.com/92877810/139740647-28c96ed8-e1d1-41c0-a87e-5cfe09a66ad7.png)

10. Click **Shipping Analysis** Page

![9-9](https://user-images.githubusercontent.com/92877810/139740648-2dba2f23-1fb0-4ee4-a60c-f05ed8c606e5.png)

ℹ️**Excercise Check!** Does your dashboard look like this screenshot?

![9-10](https://user-images.githubusercontent.com/92877810/139740649-3eb5066c-bc0c-4f33-92bd-273cda6a903a.png)

👉In our Shipping Analysis page, we prepared a variety of visualizations that will be used conjunctly with our geo map in analysis. The first chart is a bar graph of sales revenue per region. This chart is linked to our geo map and will filter regions on the geo map based on chart selection.

![9-11](https://user-images.githubusercontent.com/92877810/139740650-1138b926-7429-4796-a8f5-a5064db08a95.png)

👉The second visualization is a table displaying the No of Delivered Orders and Avg Delivery Times for stores in our shipping model. This chart has linked analysis filtering applied from our geo map and will filter entries based on selections made on our geo map.

![9-12](https://user-images.githubusercontent.com/92877810/139740651-a5c1df01-f6f0-4593-9aca-790685c2c3f7.png)

11. Scroll to the bottom

12. Select the Geo Map already created for you

![9-13](https://user-images.githubusercontent.com/92877810/139740653-c3cce88c-470d-4855-beef-65f032df0a9f.png)

13. Click **Designer** to open Builder Panel (in case not already open)

👉We want to choose a layer that will help us visualize the distribution of our measure, Average Delivery Time, in our geo visualization. The Heat Map Layer is a good way to visualize the data density of a measure on our map. Let us create this layer in our geo map

14. Click **Add Layer**

![9-14](https://user-images.githubusercontent.com/92877810/139740656-c6289226-3b2d-4b21-88d5-ebbf063d5a94.png)

15. Rename the layer to **Order Delivery Time Density**
  
👉Let us change the model for this layer to the shipping model which contains our desired measures. You can add layers sourcing measures and dimensions from multiple models on a single geo visualization, enhancing your ability to compare data.

16. Click **Select Model**

![9-15](https://user-images.githubusercontent.com/92877810/139740657-3953fc2b-4b87-4643-8ccc-9708737bf3d1.png)

17. Click **ANA260_SHIPPING_INFO**

![9-16](https://user-images.githubusercontent.com/92877810/139740659-0d771fd9-48ad-4604-94de-8f5e4ccfdf3b.png)

18. Click **OK**

![9-17](https://user-images.githubusercontent.com/92877810/139740660-3b413276-b872-47ec-9a05-d2179b097e68.png)

ℹ️SAP Analytics Cloud offers a variety of layers for geographical visualizations. The most common used ones are •Bubble Layer, which show each location as a bubble. Using color and size of the bubble allows to see correlation between different measures•Choropleth Layer, shows the shape of a geo location and allows drilling from aggregated levels such as country into smaller areas such as regions•Heat Map Layer, allows to show the concentration of geographical locationsFor your next step you like to view your data in a heat map.

19. Click **Choose Layer Type**

20. Click **Heat Map Layer**

![9-18](https://user-images.githubusercontent.com/92877810/139740661-147b4f70-4a23-47e9-95f2-9e0e2ac49878.png)

ℹ️Let us add our geo enriched dimension to this geo map.

21. Click **+ Add Location Dimension**

![9-19](https://user-images.githubusercontent.com/92877810/139740662-e84cc0e9-80d5-4c2b-b952-17521b995fa4.png)

22. Click **Store Location**

![9-20](https://user-images.githubusercontent.com/92877810/139740663-f5b60546-916d-4f31-8132-50879e0c40ba.png)

👉We want to look at Avg Delivery Time, a calculated measure in our model, to look at the density of delivery times in our heat map layer.

23. Click **Add Measure**

![9-21](https://user-images.githubusercontent.com/92877810/139740665-e19ed257-05fd-41e1-b297-18a41454414e.png)

24. Scroll and click **Avg Delivery TIme**

![9-22](https://user-images.githubusercontent.com/92877810/139740668-f9ba1595-8b2f-42aa-8d83-75602ab3954f.png)

25. Click **OK**

![9-23](https://user-images.githubusercontent.com/92877810/139740671-119deb3c-b417-4230-a435-d38b11501f2a.png)

⚠️  
Quality check! Does your geo map look like this screenshot after applying the heat map layer and zooming in?

👉Our Heat Map layer looks great, but the scale may be too large for our desired purpose. We can change the gradient properties of our heatmap to improve our visualization and make it easier to discover clusters of outlier delivery times.

![9-24](https://user-images.githubusercontent.com/92877810/139740672-46d8d7ee-57e9-420e-8907-d50d5bf28e87.png)

26. Click Edit Layer

![9-25](https://user-images.githubusercontent.com/92877810/139740673-af7bfc29-ae24-4923-a593-9b951c7c588b.png)

👉Let us reduce the blur radius so it is clearerwhere our high and low average delivery times are present in Spain. The blur radius determines the size of each data point and how it overlaps with other values. We can improve the definition between pointsby reducing the blur radius.

27. Click Expand on Avg Delivery Time

28. Change the Blue Radius from 40% to 20%

29. Click OK

![9-26](https://user-images.githubusercontent.com/92877810/139740674-1d6af52a-50d2-4dc3-85d5-a0781ca53be6.png)

⚠️Quality check! Does your geo map look like this screenshot after changing the blur radius?

![9-27](https://user-images.githubusercontent.com/92877810/139740676-d7ec6a9a-8b45-4654-ab8a-b18dc15158c9.png)

👉Let us move our geo map back to look at delivery times in **Spain**

30. Click into our Geo Map, hold and drag to be looking at **Spain**

31. Zoom into the cluster in Spain by scrolling your **mouse wheel up.**

![9-28](https://user-images.githubusercontent.com/92877810/139740677-913cba12-2116-4590-92ea-401865ec66ce.png)

👉You can change the appearance of the heat map layer as well by zooming in and out of the geo map and focusing on areas of interest. When we zoom into Spain, we notice there are some distinct clusters of higher average delivery times. Let us investigate this further.

![9-29](https://user-images.githubusercontent.com/92877810/139740678-e887acf5-1569-436d-b01b-ca9a6ee66e87.png)

👉Let us create a new layer that looks at our delivery time measuresat a store level. First, let us hide our heat map layer.

32. Click **Hide** on **Order Delivery Time Density**

33. Click **+ Add Layer**

![9-30](https://user-images.githubusercontent.com/92877810/139740680-44117c57-5680-492c-82c3-3906719b5534.png)

👉  
We are going to create a layer that shows our delivery measures on a store by store basis to further our analysis

34. Rename the layer to **Store Location Analysis**

35. Select **ANA260_SHIPPING_INFO** if not already selected

![9-31](https://user-images.githubusercontent.com/92877810/139740681-c6a17305-097e-44e5-8b44-52c00dfe8498.png)

👉We want the ability to drill up and down in our layer from a store level to an aggregated country level (i.e.Spain). Let us choose to create a choropleth layer.

36. Click **Choose Layer Type**

37. Click **Chloropleth/ Drill Layer**

![9-32](https://user-images.githubusercontent.com/92877810/139740683-1cf8dbbd-646c-4f08-b757-d4b2eafbcafd.png)

👉We can choose to use bubble instead of choropleth in the style of our drill down layer. This will represent our hierarchy members in the form of bubbles on the geo map. Since we want to look at individual stores, this is preferred!

38. Click **Choose Style**

39. Click **Bubble**

![9-33](https://user-images.githubusercontent.com/92877810/139740684-74c6c64c-d3fb-49e7-a6c4-8d734d339c20.png)

40. Click **+ Add Location Dimension** 

![9-34](https://user-images.githubusercontent.com/92877810/139740685-202beaae-18e5-41e5-ad69-c289d0690523.png)

41. Click **StoreLocation**

![9-35](https://user-images.githubusercontent.com/92877810/139740686-32d0b396-c091-4912-ae69-048947bdaf88.png)

42. Click **Add Measure/Dimension**

![9-36](https://user-images.githubusercontent.com/92877810/139740687-77ae5047-a40b-4ba7-ad6a-6ad4669c3446.png)

👉Let us add additional measures into our analysis. We can choose to color code our bubbles with the Average # of Delivered Orders to see if this measure is related to our delivery times.

43. Click **Average # of Delivered Orders**

![9-37](https://user-images.githubusercontent.com/92877810/139740690-b501aa28-9250-4d58-a31f-c8211e8fedd8.png)

44. Click **+ Add Measure**

![9-38](https://user-images.githubusercontent.com/92877810/139740691-02cad606-a063-4852-8034-81593a168c41.png)

👉We are choosing average delivery time as our bubble size, so it is easy to pinpoint which stores are outliers in our modeled data.

45. Scroll and Click **Avg Delivery Time**

![9-39](https://user-images.githubusercontent.com/92877810/139740693-91e01cb9-4f2b-426f-a632-559275622c8e.png)

⚠️Quality check! Does your geo map look like this screenshot after adding the new choropleth layer?

![9-40](https://user-images.githubusercontent.com/92877810/139740694-3a58e818-fd3a-4153-a139-7c53866a3532.png)
  
👉Based on our current geo map, the sizing of our bubbles does not suit our analysis of delivery times. We can customize how our measure is translated into bubble size to improve our visualization

46. Click **Expand** on **Avg Delivery Time**
  
👉Changing the range for our bubbles will help us identify outliers in our geo map based on our measure, Avg Delivery Time. Let us changes these ranges for the hierarchy levels we are interested in: Country, Region, and StoreLocation.

47. Expand **Range** for **Country**

48. Change upper range from **100%** to **500%**

49. Click outside the pop-up.

![9-41](https://user-images.githubusercontent.com/92877810/139740697-eddbc7a3-d29f-417a-8df8-c582acad9983.png)

50. Expand **Range** for **Region**

51. Change upper range from **100%** to **500%**

52. Click outside the pop-up.

![9-42](https://user-images.githubusercontent.com/92877810/139740699-4072727d-eacb-4129-821d-603f9d155a28.png)

53. Expand **Range** for **StoreLocation**

54. Change upper range from **100%** to **500%**

55. Click outside the pop-up.

56. Click **OK**

![9-43](https://user-images.githubusercontent.com/92877810/139740700-5e38afc4-695e-4303-8956-463a9ceb6f90.png)

⚠️Quality check! Does our geo map look like this screenshot after Bubble Size changes? It is now much easier to differentiate the hierarchy level members on our geo map.

![9-44](https://user-images.githubusercontent.com/92877810/139740701-5841516d-8007-459f-8700-3c7e6cef18be.png)

57. Click **Spain**

58. Click **Drill Down**

![9-45](https://user-images.githubusercontent.com/92877810/139740702-cfc219ba-42a9-482b-a3ee-50d1d9e03e82.png)

⚠️Quality check! Does your geo map look like this screenshot after drilling down?

👉We can see that the La Rioja region in Spain seems to have high average delivery times (with its large bubble) and high numbers ofdelivered orders. On the other hand, Castilla Leon has very low average delivery times. This is very informative, and we should look at this layer on an individual store level.

![9-46](https://user-images.githubusercontent.com/92877810/139740705-087c9288-1510-43c3-a28a-f2aa7a7d95ae.png)
  
👉Before we drill down again, let us check to see how our hierarchy is defined.

59. Click **Navigate up/down the hierarchy**

👉Let us choose the hierarchy for the current map layer we are looking at.

60. Click **Store Location**

![9-47](https://user-images.githubusercontent.com/92877810/139740706-aaafc19d-1332-44ea-8357-804cd09114aa.png)

👉As we can see, there are 2 additional hierarchy layers, Sub-Region 1 and Sub-Region 2, before we reach our desired StoreLocation level. Let us simplify our hierarchy to two levels, Country and StoreLocation, for efficiency purposes

![9-48](https://user-images.githubusercontent.com/92877810/139740708-3391394d-70d4-4ac1-93d6-af31a379db0e.png)

👉We can customize which hierarchy levels are drillable in our choropleth layer. This is a performance best practice tip! Rendering additional hierarchy levels that we are not interested in is both time and resource intensive.

61. Click the **Hierarchy** option for **Store Location Analysis**

![9-49](https://user-images.githubusercontent.com/92877810/139740710-2dee1ee5-3883-4870-8793-8504de1d4897.png)

62. Uncheck **Show Region**

63. Uncheck **Show Sub-Region 1**

64. Uncheck **Show Sub-Region 2**

65. Click **Save**

![9-50](https://user-images.githubusercontent.com/92877810/139740712-2c0cb199-32c4-4b4f-a302-9317bf8f0e40.png)
