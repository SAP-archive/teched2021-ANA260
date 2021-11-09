# Exercise 2 - Linked Analysis and Input Controls

⚠️This section builds on top of another section. If you did not complete the previous section, please select 
**“Section 1 – Creating Your First Story”** from the **“Public/TechEd”** folder and click **Copy To** your
directory. You will then be able to edit this story to complete the following exercise.

ℹ️**Objective:** Develop a basic understanding on how to make a dashboard more dynamic for your viewers to 
draw insights between multiple visualizations

**Estimated Time:** 15 mins

**Exercise Description:** In the last section, we created our first story and added new visualizations. However, 
currently our dashboard is quite static. In this section, we want to add interactive capabilities to the 
dashboard by adding new filters and input controls. This way our dashboard can be easily used by a number 
of different employees at the company - each user will be able to easily manipulate the dashboard view and 
only see what is important to them

**Key Features:**
- Learn about page filters and how to apply them to a subset of widgets only
- Understand how to add a measure and dimension input control to dynamically change the context of 
your data visualization
- Understand how to set up linked analysis to drive filters via widget interaction

⚠️**Disclaimer**
When completing exercises, some data values in the screenshots may not match what you see on your 
screen. This is because the dynamic time filters that were applied at the time the screenshots were taken is 
different from the current system date.

----------------------------------------------------------------------------------------------------------------------------------------

⚠️**Exercise Check!** Does your dashboard look like this? Are you in Edit mode?

![Image 1](https://user-images.githubusercontent.com/90856848/138132038-7cef31ce-bbb0-4a69-a906-32bf36a4b13e.png)

🚩To start off, we want to add another lane to our story where viewers can choose specific filters to apply to the page and even change measures and dimensions in charts.

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

🚩The first tool we will add to our story are page filter input controls. These allow viewers to easily change the dimensions driving the data in our visualizations on the page.
 
Let's create filters on Region and Product as these are two important dimensions that businessesuse to analyze performance.

9. Click **Page Filter**

10. Click **Dimensions**

11. Click **Region**

![img5](https://user-images.githubusercontent.com/92877810/138146758-8dd3a4cc-856b-4660-99a0-3976dc4b69d2.png)

🚩Selecting All Members in the Filter dialogue populates the input control with all members of the region dimension. This gives the person interacting with the input control the option of choosing any subset of regions. 

12. Click **All Members**

13. Click **OK**

![img6](https://user-images.githubusercontent.com/92877810/138147298-c06b17b3-49f9-4c22-acde-0f9dbc82c821.png)

⚠️Quality Check! This is what your dashboard should look like after creating the input control. 

![img7](https://user-images.githubusercontent.com/92877810/138147325-74760d6f-75b2-433e-a89b-91d0188ec329.png)

🚩You have just made a Page Filter Input Control for Region. Let us make another Page Filter for Product. 

14. Click **Insert**

15. Clicking **Insert Input Control**

![img8](https://user-images.githubusercontent.com/92877810/138147801-c8f25aab-1c1e-4c9f-961c-89826d3aa811.png)

16. Click **Dimensions**

17. Click **Product**

![img9](https://user-images.githubusercontent.com/92877810/138147803-157c49b5-3ffd-4d3a-9c99-45aeb339fc38.png)

🚩Unlike **Region, Product** has additional properties attached to it. We're interested in filtering out the product itself, so we must now select it.  

18. Click **Product (Dimension)**

![img10](https://user-images.githubusercontent.com/92877810/138147804-b8ad2528-50af-4e90-8f02-36cc38057ac1.png)

19. Click **OK**

20. Click **All Members**

![img11](https://user-images.githubusercontent.com/92877810/138147806-d8c8a1e4-5ba9-486b-b5ae-e2458fbd4ad7.png)

⚠️Quality Check! Do our Page Filter Input Controls look like this? 

🚩Now that we have a Product input control, lets focus the entire dashboard to see how we are performing when it comes to Footwear and Clothing. 

![img12](https://user-images.githubusercontent.com/92877810/138147807-2b291c88-68f5-4eb5-b1f5-a88397ba23a8.png)

21. Click **Product**

22. Click **Expand (All)**

23. Deselect **Accessories.** So only **Clothing** and **Footwear** are selected

24. Click outside to collapse the Input Control

![img13](https://user-images.githubusercontent.com/92877810/138147809-e3528f2d-b68c-425a-a234-a51a58ef376a.png)

🚩Changing the Product Input Control applies a filter to all charts and tables on the page. Now all our charts only include data for products in Clothing or Footwear. However, this behavior may be different from what we want. If we only want to change a few charts on the dashboard in response to the input control, we can do this by adding scope to our Page Filter. This is done via Linked Analysis. 

![img14](https://user-images.githubusercontent.com/92877810/138148606-f81f9d89-41e2-498a-88b7-f7532f801636.png)

25. **Right Click the Product Input Control**

26. Click **Linked Analysis**

![img15](https://user-images.githubusercontent.com/92877810/138148609-3571c0e6-209d-4760-aa8d-99fb5c9f902f.png)

ℹ️Welcome to Linked Analysis!   
  
Linked Analysis allows the user to define which widgets will be affected when interacting with the input control. 
By default an input control will be applied to all widgets on the page, but a story designer can also choose to only apply the input control to a selected set of widgets.  This is often done when one wants to compare difference slices of the data side by side.  

![img16](https://user-images.githubusercontent.com/92877810/138148611-44194bc3-2b8b-4552-955b-6cdb6971ac59.png)

🚩We only want our page filter to apply to select charts. We can select these in the Linked Analysis Panel.  

27. Click **Only Selected Widgets**

28. Click **Sales Revenue per Region for Actual**

29. Click **Gross Margin per Product, Workout Usage for Actual**

30. Click **Gross Margin per Order Date for Actual**

31. Click **Apply** 

![img17](https://user-images.githubusercontent.com/92877810/138148614-db6613fe-b2d0-4faa-b04f-a904bf659dd2.png)

🚩We can test the Linked Analysis behavior by deselecting Clothing and seeing which charts change. 

32. Click **Product**

![img18](https://user-images.githubusercontent.com/92877810/138148617-65bac5c2-36e8-42b1-9dea-89012822b289.png)

33. Deselect **Clothing**

34. Click outside to collapse the Input Control

![img19](https://user-images.githubusercontent.com/92877810/138148621-7856415c-b711-4b3f-b949-eb4ac7f3bdb4.png)

🚩Only data in the three charts we selected has changed. All other charts and tables on the page remain un-affected.  

![img20](https://user-images.githubusercontent.com/92877810/138148622-034c3b97-0511-409b-8242-af9baad4c7e0.png)

🚩Let’s revert to selecting all products. 

35. Click the **Product Input Control** 

![img21](https://user-images.githubusercontent.com/92877810/138148624-5c2feb2f-7456-4ffd-b3ab-4ee16ee4620c.png)

36. Click **(All)**

37. Click outside to collapse the Input Control

![img22](https://user-images.githubusercontent.com/92877810/138148625-5d0a8134-fb43-4392-8426-41ed3ef131aa.png)

⚠️Quality Check! Has your page reverted to show all **Products**?

![img23](https://user-images.githubusercontent.com/92877810/138148627-fc20c3b3-d3d6-4c90-b3d4-36913a5f5074.png)

🚩We can provide end users the flexibility to analyze various measures (i.e. sales revenue, gross margin, etc.) with **Measure Input Controls**. This eliminates the need to duplicate charts and allows users to dynamically change the measures each chart consumes. Let's create a Measure Input Control and direct our chart to use that instead of a single measure. 

38. Select the **Sales Revenue per Region for Actual** Chart

![img24](https://user-images.githubusercontent.com/92877810/138148628-3aa956d8-9b6d-4fea-8839-f568a4337b8f.png)

39. Click **Designer**

40. Click Remove **Sales Revenue** from **Measures**

41. Click **Add Measure**

![img25](https://user-images.githubusercontent.com/92877810/138148629-67c077c0-8da1-4485-aee4-f47d8aa95d4f.png)

42. Scroll untill **+ Create Measure Input Control** is Visible

43. Click **+ Create Measure Input Control**

![img26](https://user-images.githubusercontent.com/92877810/138149936-6301c7f5-e1cf-4639-a4c2-a99d78841fc5.png)

ℹ️Welcome to Measure Input Controls! 
  
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

🚩Please note: These input controls can be renamed; this functionality will be shown later in the styling section.  

🚩This measure input control now drives our first chart in the right lane. 

It is possible to add more than one chart to a measure input control to drive synced behavior in your story. Let's do this now and add a second chart that is controlled by this Measure Input Control.

![img30](https://user-images.githubusercontent.com/92877810/138149942-58405e25-8511-4362-8368-891c41b770bb.png)

⚠️Quality Check! This is what your dashboard should look like.  
  
Take a minute and save your work using **Ctrl + S**. 

![img31](https://user-images.githubusercontent.com/92877810/138149943-e6d5ded6-bd86-4291-9143-c2b9fc6114f2.png)

50. Click the **Gross Margin per Product, Workout Usage for Actual** Chart

51. Click **Designer**

52. Remove **Gross Margin**

53. Click **Add Measure** 

![img32](https://user-images.githubusercontent.com/92877810/138149944-1950d0dd-92dd-48d1-aae9-c2659f0370cd.png)

54. Scroll untill New Measure Input Control is Visible

55. Click **New Measure Input Control**

56. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down

![2-r1](https://user-images.githubusercontent.com/92877810/140988250-dbc6227f-991f-4b04-aed7-d34785854e42.png)

57. Click **Sales Revenue per Order Date for Actual** Chart

58. Click **Designer**

59. Remove **Sales Revenue**

![2-r2](https://user-images.githubusercontent.com/92877810/140988254-d7fc06ba-672f-4079-bf39-f64d07f7203e.png)

60. Scroll until New Measure Input Control is Visible

61. Click **New Measure Input Control**

62. Click Inside the Builder Panel to Collapse the Measure Selection Drop Down

![2-r3](https://user-images.githubusercontent.com/92877810/140988255-f33de9a9-77af-4eb9-a68c-e13db2a6a91c.png)

⚠️Quality Check! Do your story's charts use the same measures as this screenshot? 

🚩Since the measure input control is currently on Sales Revenue selection, all three of our charts are using Sales Revenue as the measure displayed in the visualization. 
  
Changing the measure input control to Gross Margin would update all 3 charts to display Gross Margin instead. 

![2-r4](https://user-images.githubusercontent.com/92877810/140988257-f1fec211-022d-4f79-bbc2-dfbab4f25691.png)

63. Click **Sales Revenue per Region for Actual** Chart

64. Remove the **Region** Dimension

65. Click **Add Dimension**

![2-r5](https://user-images.githubusercontent.com/92877810/140988259-772e2945-0f11-4c52-a5e8-b5bc50f70edb.png)

59. Scroll untill Create Dimension Input Control is Visible

60. Click **Create Dimension Input Control**

![2-r6](https://user-images.githubusercontent.com/92877810/140988260-f6427672-1494-431f-85de-5ab860c74022.png)

61. Click **Product**

62. Click **Region**

63. Click **Sales Manager**

64. Click **OK**

![2-r7](https://user-images.githubusercontent.com/92877810/140988262-d63aadd8-cbb2-4a7f-8ea4-c0ecd6b5d58d.png)

65. Click and Drag the **New Dimension Input Control** to the Left Lane

66. Drop the **Dimension Input Control Here**

![2-r8](https://user-images.githubusercontent.com/92877810/140988265-7f445aca-97cf-4adb-983f-6870fdb74bf8.png)

67. Resize the Dimension Input Control to View All Members

![2-r9](https://user-images.githubusercontent.com/92877810/140988269-0d416d50-82db-4330-8094-8ec088ebf014.png)

68. Click **Gross Margin**

69. Click **Sales Manager**

![2-r10](https://user-images.githubusercontent.com/92877810/140988270-113392d8-2132-4876-af55-81b849c0f655.png)

⚠️Quality Check! Test out the effects of measure and dimension input controls in your story.

🚩After changing both input controls, Gross Margin should be the measure displayed in every chart. The first chart now visualizes a breakdown of Gross Margin across Sales Managers rather than region. 

![2-r11](https://user-images.githubusercontent.com/92877810/140988271-162671a9-616f-4fa0-bf92-0ddc42b2c06b.png)

🚩There is still more dynamic functionality available within Sap Analytics Cloud. We can use additional functionality within Linked Analysis to link two charts so that if a data point is clicked on one chart, the other chart will update by creating a filter on that data point. Let's do this now and we'll get a better idea of what this means.  

70. Click on the **More** icon on the Gross Margin per Sales Manager per Actual Chart to Open the Context Menu

71. Click **Linked Analysis**

![2-r12](https://user-images.githubusercontent.com/92877810/140988273-0f8fd557-53e7-4a63-a81a-762b6674d6e1.png)

ℹ️Remember we're now adding linked analysis on a chart as opposed to an Input Control. This provides us with a few more options. 

72. Click **All Widgets on the Page**

73. Click **Filter on data point selection**

74. Click **Apply** 

![2-r13](https://user-images.githubusercontent.com/92877810/140988274-c1268f47-5ba7-4722-8870-e04f0661a11e.png)

🚩Let's test Linked Analysis and get some more insight on how **Gary Dumin** in performing.  

75. Click **Gary Dumin**

![2-r14](https://user-images.githubusercontent.com/92877810/140988275-1e92e97b-27c2-4e58-92b6-8771d5d29870.png)

🚩Do you see your linked charts change when highlighting a Sales Manager? Notice how the CGR in our time dimension chart is positive under this filter (Note this data may be different due to the dynamic time filter).

![2-r15](https://user-images.githubusercontent.com/92877810/140988276-260313ec-e812-4abe-8df5-9947d62f55d8.png)

76. Click within the chart to Deselect Gary

![2-r16](https://user-images.githubusercontent.com/92877810/140988277-379c5cf3-8c4c-4069-8fcf-a92167eef97f.png)

🚩Save your story by pressing **Ctrl + S**

![2-r17](https://user-images.githubusercontent.com/92877810/140988279-9f3637e9-b085-4f68-a94b-55d0a3383592.png)

⚠️Quality Check! Does your dashboard look like this screenshot?  

ℹ️You have now completed the **Linked Analysis and Input Controls** section! In this section, you have learned how to dynamically change page filters with an input control, add interactive measures and dimensions to charts also with input controls, and create powerful analytics between the charts in your story using linked analysis and data point filtering. 
  
We're going to add some styling to this dashboard later on. 

![2-r18](https://user-images.githubusercontent.com/92877810/140988282-129e4c38-5f6c-4318-ab53-e96d8d7d4a5f.png)

<br><br>

## Summary

**You have completed the entire Linked Analysis and Input Controls section!**

**You are now able to:**
- Create page filters and apply them to a subset of widgets only
- Add a measure and dimension input control to dynamically change the context of your data 
visualization
- Set up linked analysis to drive filters via widget interaction
