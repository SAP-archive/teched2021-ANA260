# Exercise 2 - Linked Analysis and Input Controls
**Exercise Check!** Does your dashboard look like this? Are you in Edit mode?

![Image 1](https://user-images.githubusercontent.com/90856848/138132038-7cef31ce-bbb0-4a69-a906-32bf36a4b13e.png)

To start off, we want to add another lane to our story where viewers can choose specific filters to apply to the page and even change measures and dimensions in charts.

1. Click the **Bottom Lane**

2. Click the **More** Action on the Lane

3. Click **Add Lane**

4. Click **Add Lane to Left**

![Image 2](https://user-images.githubusercontent.com/90856848/138132238-b0da38cb-6adb-4d07-bbe4-3446f5ffe1f3.png)

5. Click and Drag the Lane to the Left 

6. Click the **New Lane Header**  

![img3](https://user-images.githubusercontent.com/92877810/138146413-e152a26a-adef-49f8-9dee-3ef3aea5ec9a.png)

7. Click **Insert**

8. Click **Insert Input Control**

![img4](https://user-images.githubusercontent.com/92877810/138146615-59e88bff-c173-4254-a6bb-3447806c7e5c.png)

The first tool we will add to our story are page filter input controls. These allow viewers to easily change the dimensions driving the data in our visualizations on the page.
 
Let's create filters on Region and Product as these are two important dimensions that businessesuse to analyze performance.

9. Click **Page Filter**

10. Click **Dimensions**

11. Click **Region**

![img5](https://user-images.githubusercontent.com/92877810/138146758-8dd3a4cc-856b-4660-99a0-3976dc4b69d2.png)

Selecting All Members in the Filter dialogue populates the input control with all members of the region dimension. This gives the person interacting with the input control the option of choosing any subset of regions. 

12. Click **All Members**

13. Click **OK**

![img6](https://user-images.githubusercontent.com/92877810/138147298-c06b17b3-49f9-4c22-acde-0f9dbc82c821.png)

Quality Check! This is what your dashboard should look like after creating the input control. 

![img7](https://user-images.githubusercontent.com/92877810/138147325-74760d6f-75b2-433e-a89b-91d0188ec329.png)

You have just made a Page Filter Input Control for Region. Let us make another Page Filter for Product. 

14. Click **Insert**

15. Clicking **Insert Input Control**

![img8](https://user-images.githubusercontent.com/92877810/138147801-c8f25aab-1c1e-4c9f-961c-89826d3aa811.png)

16. Click **Dimensions**

17. Click **Product**

![img9](https://user-images.githubusercontent.com/92877810/138147803-157c49b5-3ffd-4d3a-9c99-45aeb339fc38.png)

Unlike **Region, Product** has additional properties attached to it. We're interested in filtering out the product itself, so we must now select it.  

18. Click **Product (Dimension)**

![img10](https://user-images.githubusercontent.com/92877810/138147804-b8ad2528-50af-4e90-8f02-36cc38057ac1.png)

19. Click **OK**

20. Click **All Members**

![img11](https://user-images.githubusercontent.com/92877810/138147806-d8c8a1e4-5ba9-486b-b5ae-e2458fbd4ad7.png)

Quality Check! Do our Page Filter Input Controls look like this? 

Now that we have a Product input control, lets focus the entire dashboard to see how we are performing when it comes to Footwear and Clothing. 

![img12](https://user-images.githubusercontent.com/92877810/138147807-2b291c88-68f5-4eb5-b1f5-a88397ba23a8.png)

21. Click **Product**

22. Click **Expand (All)**

23. Deselect **Accessories.** So only **Clothing** and **Footwear** are selected

24. Click outside to collapse the Input Control

![img13](https://user-images.githubusercontent.com/92877810/138147809-e3528f2d-b68c-425a-a234-a51a58ef376a.png)

Changing the Product Input Control applies a filter to all charts and tables on the page. Now all our charts only include data for products in Clothing or Footwear. However, this behavior may be different from what we want. If we only want to change a few charts on the dashboard in response to the input control, we can do this by adding scope to our Page Filter. This is done via Linked Analysis. 

![img14](https://user-images.githubusercontent.com/92877810/138148606-f81f9d89-41e2-498a-88b7-f7532f801636.png)

25. **Right Click the Product Input Control**

26. Click **Linked Analysis**

![img15](https://user-images.githubusercontent.com/92877810/138148609-3571c0e6-209d-4760-aa8d-99fb5c9f902f.png)

Welcome to Linked Analysis! 
  
  
Linked Analysis allows the user to define which widgets will be affected when interacting with the input control. 
By default an input control will be applied to all widgets on the page, but a story designer can also choose to only apply the input control to a selected set of widgets.  This is often done when one wants to compare difference slices of the data side by side.  

![img16](https://user-images.githubusercontent.com/92877810/138148611-44194bc3-2b8b-4552-955b-6cdb6971ac59.png)

We only want our page filter to apply to select charts. We can select these in the Linked Analysis Panel.  

27. Click **Only Selected Widgets**

28. Click **Sales Revenue per Region for Actual**

29. Click **Gross Margin per Product, Workout Usage for Actual**

30. Click **Gross Margin per Order Date for Actual**

31. Click **Apply** 

![img17](https://user-images.githubusercontent.com/92877810/138148614-db6613fe-b2d0-4faa-b04f-a904bf659dd2.png)

We can test the Linked Analysis behavior by deselecting Clothing and seeing which charts change. 

32. Click **Product**

![img18](https://user-images.githubusercontent.com/92877810/138148617-65bac5c2-36e8-42b1-9dea-89012822b289.png)

33. Deselect **Clothing**

34. Click outside to collapse the Input Control

![img19](https://user-images.githubusercontent.com/92877810/138148621-7856415c-b711-4b3f-b949-eb4ac7f3bdb4.png)

Only data in the three charts we selected has changed. All other charts and tables on the page remain un-affected.  

![img20](https://user-images.githubusercontent.com/92877810/138148622-034c3b97-0511-409b-8242-af9baad4c7e0.png)

Let’s revert to selecting all products. 

35. Click the **Product Input Control** 

![img21](https://user-images.githubusercontent.com/92877810/138148624-5c2feb2f-7456-4ffd-b3ab-4ee16ee4620c.png)

36. Click **(All)**

37. Click outside to collapse the Input Control

![img22](https://user-images.githubusercontent.com/92877810/138148625-5d0a8134-fb43-4392-8426-41ed3ef131aa.png)

Quality Check! Has your page reverted to show all **Products**?

![img23](https://user-images.githubusercontent.com/92877810/138148627-fc20c3b3-d3d6-4c90-b3d4-36913a5f5074.png)

We can provide end users the flexibility to analyze various measures (i.e. sales revenue, gross margin, etc.) with **Measure Input Controls**. This eliminates the need to duplicate charts and allows users to dynamically change the measures each chart consumes. Let's create a Measure Input Control and direct our chart to use that instead of a single measure. 

38. Select the **Sales Revenue per Region for Actual** Chart

![img24](https://user-images.githubusercontent.com/92877810/138148628-3aa956d8-9b6d-4fea-8839-f568a4337b8f.png)

39. Click **Designer**

40. Click Remove **Sales Revenue** from **Measures**

41. Click **Add Measure**

![img25](https://user-images.githubusercontent.com/92877810/138148629-67c077c0-8da1-4485-aee4-f47d8aa95d4f.png)

42. Scroll untill **+ Create Measure Input Control** is Visible

43. Click **+ Create Measure Input Control**

![img26](https://user-images.githubusercontent.com/92877810/138149936-6301c7f5-e1cf-4639-a4c2-a99d78841fc5.png)

Welcome to Measure Input Controls! 
  
Measure Input Controls are a great way to change the Measure that is represented on a chart at view time. If your viewer would rather see Gross Margin in the regional breakdown than Sales Revenue, a Measure Input Control provides this functionality. 

![img27](https://user-images.githubusercontent.com/92877810/138149938-bce78603-ea33-4d36-8ef6-c847b242f979.png)

44. Click **Sales Revenue**

45. Click **Gross Margin**

46. Click **OK**

![img28](https://user-images.githubusercontent.com/92877810/138149939-105526b5-2013-4d58-8307-35ec09d83dd0.png)

47. Click and Drag the **New Measure Input Control** to the Left Lane

48. Drop the **Measure Input Control** Here

![img29](https://user-images.githubusercontent.com/92877810/138149941-83973de8-4bc0-4302-a5cc-97753d069bfd.png)

49. Resize the Measure Input Control to see all members

Please note: These input controls can be renamed; this functionality will be shown later in the styling section.  

This measure input control now drives our first chart in the right lane. 

It is possible to add more than one chart to a measure input control to drive synced behavior in your story. Let's do this now and add a second chart that is controlled by this Measure Input Control.

![img30](https://user-images.githubusercontent.com/92877810/138149942-58405e25-8511-4362-8368-891c41b770bb.png)

Quality Check! This is what your dashboard should look like.  
  
Take a minute and save your work using **Ctrl + S**. 

![img31](https://user-images.githubusercontent.com/92877810/138149943-e6d5ded6-bd86-4291-9143-c2b9fc6114f2.png)

50. Click the **Gross Margin per Product, Workout Usage for Actual** Chart

51. Remove **Gross Margin**

52. Click **Add Measure** 

![img32](https://user-images.githubusercontent.com/92877810/138149944-1950d0dd-92dd-48d1-aae9-c2659f0370cd.png)

53. Scroll untill New Measure Input Control is Visible

54. Click **New Measure Input Control**

55. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down

![img33](https://user-images.githubusercontent.com/92877810/138149945-0cd758f0-232f-49c8-9abc-725e750c05ab.png)

Quality Check! Do your story's charts use the same measures as this screenshot? 

Since the measure input control is currently on Sales Revenue selection, all three of our charts are using Sales Revenue as the measure displayed in the visualization. 
  
Changing the measure input control to Gross Margin would update all 3 charts to display Gross Margin instead. 

![img34](https://user-images.githubusercontent.com/92877810/138149947-54aaadde-cb43-4b88-9a02-cf9dab0ceed8.png)

56. Click **Sales Revenue per Region for Actual** Chart

57. Remove the **Region** Dimension

58. Click **Add Dimension**

![img35](https://user-images.githubusercontent.com/92877810/138149948-33882713-8a85-459f-8599-502fee2c8812.png)

59. Scroll untill Create Dimension Input Control is Visible

60. Click **Create Dimension Input Control**

![img36](https://user-images.githubusercontent.com/92877810/138149949-b1fdc670-3177-4d54-a755-8ed1b480d67b.png)

61. Click **Product**

62. Click **Region**

63. Click **Sales Manager**

64. Click **OK**

![img37](https://user-images.githubusercontent.com/92877810/138149950-0669b426-50f0-4d9d-95d2-27e9fb98a860.png)

65. Click and Drag the **New Dimension Input Control** to the Left Lane

66. Drop the **Dimension Input Control Here**

![img38](https://user-images.githubusercontent.com/92877810/138149951-ce65144a-7bfe-4de6-aef3-c1fc9a1664f0.png)

67. Resize the Dimension Input Control to View All Members

![img39](https://user-images.githubusercontent.com/92877810/138149952-f02c5d3f-a660-49c7-95d5-6dfb146de93a.png)

68. Click **Gross Margin**

69. Click **Sales Manager**

![img40](https://user-images.githubusercontent.com/92877810/138149953-1a55fd87-6039-4792-8743-958f027f212f.png)

Quality Check! Test out the effects of measure and dimension input controls in your story.

After changing both input controls, Gross Margin should be the measure displayed in every chart. The first chart now visualizes a breakdown of Gross Margin across Sales Managers rather than region. 

![img41](https://user-images.githubusercontent.com/92877810/138149955-8deee799-258e-42e7-b00c-65deba6df177.png)

There is still more dynamic functionality available within Sap Analytics Cloud. We can use additional functionality within Linked Analysis to link two charts so that if a data point is clicked on one chart, the other chart will update by creating a filter on that data point. Let's do this now and we'll get a better idea of what this means.  

70. Click on the **More** icon on the Gross Margin per Sales Manager per Actual Chart to Open the Context Menu

71. Click **Linked Analysis**

![img42](https://user-images.githubusercontent.com/92877810/138149956-18d558ea-8774-4f29-b879-ea893d195e7f.png)

Remember we're now adding linked analysis on a chart as opposed to an Input Control. This provides us with a few more options. 

72. Click **All Widgets on the Page**

73. Click **Filter on data point selection**

74. Click **Apply** 

![img43](https://user-images.githubusercontent.com/92877810/138149959-789c6dbe-dbe4-4ee3-ac4a-c2fc4ab7d82e.png)

Let's test Linked Analysis and get some more insight on how **Gary Dumin** in performing.  

75. Click **Gary Dumin**

![img44](https://user-images.githubusercontent.com/92877810/138149961-96df2d23-a8b1-49c2-8622-824c76566fa7.png)

Do you see your linked charts change when highlighting a Sales Manager? Notice how the CGR in our time dimension chart is positive under this filter (Note this data may be different due to the dynamic time filter).

![img45](https://user-images.githubusercontent.com/92877810/138149962-8cbec171-e519-4d68-b613-9daca5f3cb16.png)

76. Click within the chart to Deselect Gary

![img46](https://user-images.githubusercontent.com/92877810/138149963-129790a6-fe35-4b58-b15b-b46c649b7b8c.png)

Save your story by pressing **Ctrl + S**

![img47](https://user-images.githubusercontent.com/92877810/138149965-f38d924e-c107-43d8-89f1-45ca82d390ed.png)

Quality Check! Does your dashboard look like this screenshot?  

You have now completed the **Linked Analysis and Input Controls** section! In this section, you have learned how to dynamically change page filters with an input control, add interactive measures and dimensions to charts also with input controls, and create powerful analytics between the charts in your story using linked analysis and data point filtering. 
  
We're going to add some styling to this dashboard later on. 

![img48](https://user-images.githubusercontent.com/92877810/138149968-c8ef67f0-442e-4815-9258-e8dcfe16b985.png)

