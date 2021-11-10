# Section 8 - Calculations and Blending

ℹ️**Objective:** Use the latest calculations available in SAP Analytics Cloud to expose additional information that 
was not available in your original data model. Understand the potential and workflow of blending models and 
creating calculations in our story.

**Estimated Time:** 25 mins

**Exercise Description:** You have access to shipping information and financial sales data that with some 
common dimensions, including Order Number and Store Name. You need to create various calculated 
dimensions, statistical aggregations, and blended visualizations to understand the effects of shipping times 
and impact of delivery delays on sales revenue.

**Key Features:**
- Create calculated dimensions with string functions to enhance your data
- Understand how to blend data models by linking on common dimensions
- Employ statistical calculations in aggregations of your data
- Integrate calculation input controls to simulate values in your visualizations

⚠️**Disclaimer**
When completing exercises, some data values in the screenshots may not match what you see on your 
screen. This is because the dynamic time filters that were applied at the time the screenshots were taken is 
different from the current system date.

----------------------------------------------------------------------------------------------------------------------------------------


⚠️Does your Dashboard look like this?

1. Click the **Main Menu** icon

![8-1](https://user-images.githubusercontent.com/92877810/141006651-c61908cf-8b21-4d12-96c8-323b0ffc92e1.png)

2. Click **Files**

![8-2](https://user-images.githubusercontent.com/92877810/141006655-b009af92-d530-42ea-9576-b8c0b8dcc1bd.png)

3. Click **Public**

![8-3](https://user-images.githubusercontent.com/92877810/141006657-5077c01f-82cb-4db0-ba11-3811853726e4.png)

4. Click **TechEd 2021**

![8-4](https://user-images.githubusercontent.com/92877810/141006659-58e0878e-3268-4c09-bca5-266cc16c467f.png)

5. Select **Section 8.0 - Calculations and Blending (Start)** 

6. Click **Copy** icon

![8-5](https://user-images.githubusercontent.com/92877810/141006662-c085bfe9-084f-406a-9ccb-3776955a7405.png)

🚩Save the file in **MyFiles**

7. Save the file as **"ANA260_Section 8_Your Initials"**

8. Click **OK**

![8-6](https://user-images.githubusercontent.com/92877810/141006664-f993b933-5fc0-442d-9ed5-08bccfeb2883.png)

9. Click **MyFiles**

![8-7](https://user-images.githubusercontent.com/92877810/141006666-28635412-5785-44ac-b1fd-e16315dc4be1.png)

10. Click **ANA260_Section 8_Your Initials**

![8-8](https://user-images.githubusercontent.com/92877810/141006667-985189c7-9788-487a-8064-a06f5158e39b.png)

11. Click **Edit** 

![8-9](https://user-images.githubusercontent.com/92877810/141006670-96651307-8ca9-4bfa-99a0-2eb8adcdfb5b.png)

12. Click **Operations Overview**

![8-10](https://user-images.githubusercontent.com/92877810/141006671-45a49347-3add-497c-ae5e-05d5cbf1b75b.png)

⚠️Exercise check! Does your dashboard look like this screenshot in Edit mode? 

![8-11](https://user-images.githubusercontent.com/92877810/141006673-3826b6bd-9bf0-4d51-8424-7612626c6275.png)

🚩When working with your data in SAP Analytics Cloud, you may find that you want to look at additional components to your data that are currently not captured by the existing measures and dimensions in the model. Luckily, story designers can extend the data models with additional calculated measures and dimensions. This enables the story creator to delve into further insights from their data. Let us start by creating a calculated dimension that divides the Store dimension in our data into Studios and Non-Studios. 

13. Click **Gross Margin % for Actual** Chart

![8-12](https://user-images.githubusercontent.com/92877810/141006677-0d6bbe2e-d1bf-43bb-9974-32056994bc67.png)

14. Click **Designer**

15. Click **+ Add Dimension**

![8-13](https://user-images.githubusercontent.com/92877810/141006679-c4ddfcc8-ad52-4ed0-acf1-f4c75a6b601d.png)

16. Scroll and Click **+ Create Calcluated Dimension...**

![8-14](https://user-images.githubusercontent.com/92877810/141006681-e1068697-44ba-4718-99b7-83fb9ee468da.png)

ℹ️Welcome to Calculated Dimensions!  
  
Calculated Dimensions are useful when you want to enrich your dimension if your model does not have the needed format. 
 
You can choose to combine existing dimensions to create your own dimensions. There are two calculated dimensions that can be created: 
  
**Calculated Dimension:** Use formulas to create new dimension members 
  
**Measure Based Dimension:** Use ranges within an existing measure to determine how to group 
dimension members together 

![8-15](https://user-images.githubusercontent.com/92877810/141006683-1dac0f5e-40f5-42b1-9448-84903c584235.png)

🚩As we want to identify the stores that are studios, we will use the regular calculated dimension. 

17. Click **Calculated DImension**

![8-16](https://user-images.githubusercontent.com/92877810/141006684-629e5566-31ab-4431-afcd-6fc004c70b94.png)

🚩The formula field for Calculated Dimensions uses conditional logic and function formulas to create the Dimension rules. This offers the business analyst great flexibility in defining new calculated dimensions. 

18. Press **Ctrl + Space** on the Keyboard

![8-17](https://user-images.githubusercontent.com/92877810/141006687-22d5b394-0876-4870-a982-91d0838a5f94.png)

19. Click IF

🚩Our IF statement has three fields. The first field is used as a condition that evaluates to true or false. The second field is the Dimension value if True and the third field is the Dimension value if False. 

![8-18](https://user-images.githubusercontent.com/92877810/141006690-43289132-1d4a-4003-9185-c48ed9272b85.png)

20. Click the **Condition (First Field)** in the IF Formula

![8-19](https://user-images.githubusercontent.com/92877810/141006691-5ff882ef-e972-42a5-8b2b-df41ecf3f497.png)

21. Press **Ctrl + Space** on the Keyboard
  
💡Using Ctrl + Space is a great way to learn how to use the Calculation Editor. Using this hotkey combination will always bring up all possible functions and measures/dimensions that can be typed into the according field for the ease of the user. 

![8-20](https://user-images.githubusercontent.com/92877810/141006692-1b3a8569-4491-4d14-b203-2fc7918a041b.png)

ℹ️Welcome to String Functions in the Calculation Editor! There are a variety of different String Functions that can be used to transform the Dimension values to a specific use case. 
  
**FINDINDEX:** Search for a substring and return its 0 based index 
**ENDSWITH:** Returns True if given string ends with user given substring 
**TRIM:** Removes unwanted leading and trailing spaces 
**REPLACE:** Replace characters in a string with a specified replacement 
**SPLIT:** Returns substring from a string using a specified divider 
**UPPERCASE/LOWERCASE:** Convert a string to all Lower or all Upper case 
**CONCAT:** Combine two strings together 
**LEFT/RIGHT:** Returns the specified number of characters from the beginning or end of a string 
  
Let us use RIGHT function to categorize Stores by if they are a Studio. 

22. Scroll till **RIGHT** is **Visible**

23. Click **RIGHT**

![8-21](https://user-images.githubusercontent.com/92877810/141006695-8a2018bd-3e34-455f-a47c-e8fd45b3c6dd.png)

🚩Here we are specifying the Dimension we are reading our string from

24. Type **St** in the **First Input Field** for **RIGHT**

25. Click **Store**

![8-22](https://user-images.githubusercontent.com/92877810/141006697-d73c223a-8627-4d41-a7a0-3a9ce1a7198a.png)

ℹ️Since Dimensions often have an ID and 
Description, it is important to clarify that we are looking to parse the Store name from description here. 

26. Type in a **Period "."**

27. Press **Ctrl + Space** on the keyboard

28. Click **Description**

![8-23](https://user-images.githubusercontent.com/92877810/141006698-bc5592b2-9763-471b-980f-fd1b0530659f.png)

🚩We know we are trying to divide our Store dimension into Studios and Non-Studio. Since we are looking for "Studio" at the end of store name, we know we should filter on 6 characters using our RIGHT string function. 

29. Type **"6"** in the **Second Input Field** for the **RIGHT** Function

![8-24](https://user-images.githubusercontent.com/92877810/141006700-9275c240-e159-478e-b613-2334cb849a77.png)

🚩Let us compare the last 6 letters of our store name with Studio to group them into two Store Groups. 

30. Type in =**"Studio"** following the RIGHT formula

31. Type in **"Studio"** in the **TRUE** Field for the IF Function

32. Type in **"Non-Studio"** in the **FALSE** Field for the  IF Function

![8-25](https://user-images.githubusercontent.com/92877810/141006702-74aad9f1-5737-44d0-81ed-cb6481387cdc.png)

⚠️Quality Check! Does the end of your formula look like this? 

![8-26](https://user-images.githubusercontent.com/92877810/141006703-ac58bbb8-b21d-4bdd-8e61-bc4147c337ea.png)

🚩Format will parse your Formula and identify if there are any problems with the input parameters. 

33. Click **Format** to Validate the Formula
  
🚩Great! Our formula is valid and good for use in defining a new Calculated Dimension. Let us name this Dimension and use it in our charts. 

![8-27](https://user-images.githubusercontent.com/92877810/141006705-223073c3-2bf1-4b4e-801a-4a3b5d499aee.png)

34. Name the Calculated Dimension as **Store Group**

35. Click **OK**

![8-28](https://user-images.githubusercontent.com/92877810/141006707-c60f5381-be9e-463d-9a82-5e7b37d045dc.png)

⚠️Quality check! Does your chart look like this after including your Calculated Dimension? 

🚩By creating a Calculated Dimension, we are able extract further insights from our data. We can now see that Gross Margin % is higher for Studios than other stores. This could be of interest to us for further financial analysis and investments. 

![8-29](https://user-images.githubusercontent.com/92877810/141006708-2ba13a1f-b302-4b12-b4f3-1ba783cbf162.png)

🚩Let us use our new Calculated Dimension to find out the split of Average Sales Revenue by Store Group. 

36. Click Avg Sales Revenue for Actual Chart

![8-30](https://user-images.githubusercontent.com/92877810/141006711-b0215de9-3334-4faa-93ce-1087c3755f0b.png)

37. Click **+ Add Dimension** 

![8-31](https://user-images.githubusercontent.com/92877810/141006713-6fc3679d-96a2-4405-b87e-2f0bc6de0f0d.png)

38. Scroll and Click **Store Group**

39. Click Inside the Builder Panel to Collapse the Dimension Selection Drop Down Menu 

![8-32](https://user-images.githubusercontent.com/92877810/141006714-7dfdceba-e915-40a4-99f5-bd6b0c3de334.png)

⚠️Quality check! Do your charts look like this screenshot? 
  
🚩We can now see that Avg Sales Revenue is also higher for Studio Stores. It could be a good business decision to change our contract structure with our Studio Stores! 

![8-33](https://user-images.githubusercontent.com/92877810/141006715-991c052d-6d0b-4758-9789-ae58619b8d1e.png)

🚩Up until this point, we have been working with visualizations built from measures and dimensions spanning a single model. Now, we can improve the value of our analysis through Blending to combine data sources. We can accomplish this by linking dimensions across models so we can compare and analyze the relationship between measures and dimensions across multiple models

ℹ️If you are missing the icon for Link Dimensions in your toolbar, click on 
... under More to surface this option. 

40. Click **Link Dimensions**

![8-34](https://user-images.githubusercontent.com/92877810/141006717-6b4b2378-c714-4f7c-8254-0355efba9097.png)

ℹ️Welcome to Link Dimensions! 
  
Link Dimensions allow you to create blended visualizations that display data from multiple models. It also allows you to create filters that simultaneously update all visualization that include linked data regardless of the model.  
  
By default, the ID attribute is used to match members between the linked dimensions. However, for non-hierarchy dimensions it is possible to change the description that is used for linking. 

We can utilize Linked Dimensions in our data by linking across the Finance and Shipping models by connecting dimensions that are identical across our two models. 

![8-35](https://user-images.githubusercontent.com/92877810/141006720-9ea97ba9-0c97-4dd3-99c0-06ab53b26309.png)

🚩Let us link the Order Number and Store dimensions between our two models. Both these dimensions are identical across our models and have independent members that we can gather insights from. By linking on Store and Order Number we can look at analyses that target Store entities or individual orders. 

41. Scroll and Click **Order Number**
 
42. Scroll and Click **Order Number**
 
![8-36](https://user-images.githubusercontent.com/92877810/141006722-8587b3cd-b56c-48b1-884b-e315016e4c82.png)

43. Scroll and Click **Store** 
 
44. Scroll and Click **Store**
 
![8-37](https://user-images.githubusercontent.com/92877810/141006724-2ee1cb5a-43dc-4634-a3bc-4ab37e0da50b.png)

🚩It is important to specify the Dimension Attribute we are linking across. Order Number in our models is common on the Dimension ID whereas Store is common on the Dimension Description (the store name). Let us make sure that Order Number is linked by IDs between the models and Store is linked by Description or Store Names between the models. 

45. Click **Link Attribute**

46. Click **ID**

![8-38](https://user-images.githubusercontent.com/92877810/141006726-e32881f7-4d96-4b1b-bbab-aed1ac9db005.png)

47. Click **Link Attribute**

48. Click **ID**

![8-39](https://user-images.githubusercontent.com/92877810/141006729-39ceac93-9b20-4a10-8114-d9d232872345.png)

49. Click **Link Attribute**

50. Click **Description**

![8-40](https://user-images.githubusercontent.com/92877810/141006731-dfd107d6-651f-43eb-8632-774dd5873b77.png)

51. Click **Link Attribute**

52. Click **Description**

53. Click **Set**

![8-41](https://user-images.githubusercontent.com/92877810/141006732-a25a1567-4da0-43e9-83f1-ab936ec2b0d6.png)

🚩SAP Analytics Cloud will display the model links you have created to link dimensions. We could choose to edit these links or add more linked dimensions. 

54. Click **Done**

![8-42](https://user-images.githubusercontent.com/92877810/141006734-6795f708-f8c7-4c92-af8e-97fc8d2c25ae.png)

🚩Now that we have Linked Dimensions, we can create blended visualizations to look at correlations in our data. As a business analyst, we may be concerned about shipping delays and how it affects our company revenue. Let us look at a blended table to display information that would help this analysis

55. Scroll to the Right of the Dashboard

56. Click **ANA260_Shipping_Info** Table

![8-43](https://user-images.githubusercontent.com/92877810/141006735-34185c59-ebba-4122-837c-db609b72e3fe.png)

57. Click **+ Add Linked Models**

![8-44](https://user-images.githubusercontent.com/92877810/141006736-0e31025f-79e6-41ce-a5af-919dd8c2b05f.png)

58. Click **ANA260_ORDER_FINANCE**

ℹ️We are now able to see ANA260_ORDER_FINANCE as a linkable model to this table because we have linked it to our Shipping model on Order Number and Store dimensions. 
  
We can choose to display measures and calculations across our columns from both models to look at the relationships in the data. 
  
In this table, we have specified Reasons for Delay as our Row dimension. We can look at how our Finance data is affected in each of these delay members. 

![8-45](https://user-images.githubusercontent.com/92877810/141006738-5f189140-81fb-48c7-91cb-7a5afbbe90bd.png)

🚩Let us create a calculation using Finance data to see how much of our product revenue falls under each of the Reasons for Delay categories. 

59. Click the **More Action** Icon for the **Account Dimension**

60. Click **Add Calculation**

61. Click **ANA260_ORDER_FINANCE**

![8-46](https://user-images.githubusercontent.com/92877810/141006741-e6b3e9cc-67c2-465f-9d93-e4216a849bf9.png)

62. Rename the Calculation to % **Contribution to Revenue**

![8-47](https://user-images.githubusercontent.com/92877810/141006743-03c9e2bd-e718-43aa-8278-ebb51825ab5b.png)

63. Type in "%" in Edit Formula

64. Select **%GrandTotal**

![8-48](https://user-images.githubusercontent.com/92877810/141006745-386f4b59-bc8e-4277-8e22-b8af9e836642.png)

65. Type in **"Re"** in %GrandTotal Field

66. Click **["ANA260_ORDER_FINANCE":Sales_Revenue]** 

67. Click **OK**

![8-49](https://user-images.githubusercontent.com/92877810/141006746-af20207b-5151-4991-b6d3-343151979f1c.png)

🚩Our table has updated with this calculation, but it has also included many other measures from the Finance model. First, we need to filter what columns are included in the table. 

68. Click **Filter**

69. Click **ANA260_ORDER_FINANCE**

![8-50](https://user-images.githubusercontent.com/92877810/141006749-67804dab-14de-45aa-b737-282d2253f339.png)

70. Scroll and Click **% Contribution to Revenue**

71. Click **OK**

![8-51](https://user-images.githubusercontent.com/92877810/141006750-8f335f7a-f778-42d6-9e67-15730d3ab06b.png)

⚠️Quality Check! Does your table look like this screenshot? 

🚩We can see how useful blended visualizations can be with multiple data sets. From this table, we can see that around 42% of our revenue ships on time. However, weather conditions and out of stock also have relatively high % contributions to revenue. We should probably consider inventory management improvements as over 12% of our revenue in shipments are delayed due to being Out of Stock. 

![8-52](https://user-images.githubusercontent.com/92877810/141006755-d776d870-e316-4974-95f8-0a372f7d6c4f.png)

🚩We can create calculations with measures from both models for visualization purposes. Let us look at the relationship between average order size from our stores and the delivery time

72. Scroll down 

73. Click the **Store Order Size per Store for Actual** Chart

![8-53](https://user-images.githubusercontent.com/92877810/141006756-ee72e780-d22a-4d6d-b58f-f6f71ace03ff.png)

🚩Once again, our visualization has a linked model for Finance. Let us add a new measure for Store Order Size. 

74. Click **Add Measure** 

![8-54](https://user-images.githubusercontent.com/92877810/141006759-bd68fa6b-1b9b-4ec8-8e05-89733a053cc9.png)

75. Click **ANA260_SHIPPING_INFO**
 
![8-55](https://user-images.githubusercontent.com/92877810/141006761-0605aa7b-a50a-4484-9501-104a19fd174c.png)

76. Click **Store Order Size**

77. Click Inside the Builder Panel to collapse the Measure Selection drop - down menu 

![8-56](https://user-images.githubusercontent.com/92877810/141006763-db21276f-c911-4600-ab86-4e40874d5c3d.png)

⚠️Quality check! Does your chart appear like this screenshot? 
 
**Note:** You might have a different color chart

![8-57](https://user-images.githubusercontent.com/92877810/141006766-e254012f-097d-40aa-aa53-be233180b610.png)

ℹ️Let us look at how this calculation was created. We can easily examine the formula by going into the options

78. Click **More Action** Icon for **Store Order Size**

79. Click **Edit Calculation**

![8-58](https://user-images.githubusercontent.com/92877810/141006767-f447fa44-ee3b-4041-810c-af7cf37e4d52.png)

🚩Here is the formula for Store Order Size. It is a calculation using Sales Revenue from the Finance model and a Count 
Aggregation from the Shipping Model for the Number of Delivered Orders. Since we are blending on Store name, our chart will understand this context for our Shipping aggregation. 

80. Click **OK**

![8-59](https://user-images.githubusercontent.com/92877810/141006768-980bec32-9d34-44a5-a7b6-965feca41b88.png)

🚩Let us use a Top N ranking to sort our chart data since we are interested in analyzing our top performing stores rather than all our stores. 

81. Click **More Actions**

82. Click **Rank**

83. Click **Top N Options**

![8-60](https://user-images.githubusercontent.com/92877810/141006773-9480f8c6-e083-4c76-9c51-1153b83d2a7e.png)

84. Set Value to 10

85. Click **Apply**

![8-61](https://user-images.githubusercontent.com/92877810/141006775-d8848aa5-b409-4401-81a3-df79a30b9f11.png)

⚠️Quality check! Does your chart look like this screenshot? 

![8-62](https://user-images.githubusercontent.com/92877810/141006777-18f8210e-3b20-45a7-91e0-c50d2610b4f7.png)

🚩We want to use this chart to drive our analysis to be able to filter on a top performing store. Let us use Linked Analysis from this chart to filter other visualizations. 

86. Click **More Actions**

87. Click **Linked Analysis**

![8-63](https://user-images.githubusercontent.com/92877810/141006779-74abb924-368d-416b-b74b-e0e8a3ece9a8.png)

🚩We want to select which visualizations are impacted by filtering when we select a top performing store. Let us choose only selected widgets for Linked Analysis. 

88. Click Only **Selected Widgets**

![8-64](https://user-images.githubusercontent.com/92877810/141006780-3e982569-4cb6-4385-866e-6cc90e345c70.png)

🚩Let us link our blended chart to a chart that 
only uses the Shipping model. Any selections on our original chart will filter to the secondary chart via Store name. 

89. Scroll and Click **Avg Delivery Time per Store for Actual**

90. Click **Apply** 

![8-65](https://user-images.githubusercontent.com/92877810/141006781-64a8ad43-e637-443d-b956-a71e76aab5ec.png)

91. Click the First Three Entries in the Store Order Size per Store Chart

![8-66](https://user-images.githubusercontent.com/92877810/141006783-9058473a-f798-4a28-a51a-eec203f70750.png)

92. Click **Filter**

![8-67](https://user-images.githubusercontent.com/92877810/141006785-1e03fbb0-2508-4437-88bd-2e5897d44ca1.png)

⚠️Quality check! Do your two charts look like this screenshot? 
 
**Note:** You might have a different color for your first chart.
  
🚩It looks as if there is a relationship between larger average order size and a faster average delivery. We have filtered using Linked Analysis from our Finance model with Store Order Size to our Shipping model with Avg Delivery Time based on the linking of dimensions we have created previously. 
  
Let us now look a scatterplot to see if Average Delivery Time is affecting our Gross Margin. 

![8-68](https://user-images.githubusercontent.com/92877810/141006786-7bbc3a60-b04f-4924-b782-bb371a3fda84.png)

93. Scroll to the right of the dashboard

94. Click **Avg Delivery Time. Gross Margin per Store for Actual Chart**

![8-69](https://user-images.githubusercontent.com/92877810/141006788-d9f9a577-ee31-4542-a026-9b4775c5be1f.png)

🚩Scatterplots are a great way to look at the correlation between two measures in our blended data. We will be comparing the average delivery time and gross margin for each store. Let us move to the Builder panel. 

95. Click **Add Measure**

![8-70](https://user-images.githubusercontent.com/92877810/141006790-e5b8e778-9961-4e3d-a4d1-aef5dba33b22.png)

96. Click **ANA260_SHIPPING_INFO**

![8-71](https://user-images.githubusercontent.com/92877810/141006793-4c724e69-1371-44d1-9d07-990e04da8da2.png)

97. Click **Avg Delivery Time**

![8-72](https://user-images.githubusercontent.com/92877810/141006794-c38b5d14-441d-492d-8564-973e6f4ff29d.png)

98. Click **Add Measure**

![8-73](https://user-images.githubusercontent.com/92877810/141006795-cd41d4da-3739-47f7-92df-8fb36f032f85.png)

99. Click **ANA260_ORDER_FINANCE**

![8-74](https://user-images.githubusercontent.com/92877810/141008238-9739cec0-38c6-41a7-b3ae-bb4211785765.png)

100. Click **Gross Margin**

![8-75](https://user-images.githubusercontent.com/92877810/141008240-7f924e57-0e99-4d26-8670-16176ad3a29d.png)

⚠️Quality check! Does your scatterplot look like this screenshot? We can see that stores with higher avg delivery time seem to also have lower gross margin

![8-76](https://user-images.githubusercontent.com/92877810/141008241-64e2afa0-70d8-4e87-83ec-0e263365f0bc.png)

🚩Let us now test out Calculation Input Controls and simulating values. Here we have a basic financial statement of gross margin, sales revenue, and cost of goods sold calculated by the difference between sales revenue and gross margin. We want to simulate what our gross margin % on each product would be given a simulated sales revenue increase

101. Scroll to the bottom of the Dashboard

102. Click the **ANA260_ORDER_FINANCE** Table

![8-77](https://user-images.githubusercontent.com/92877810/141008242-8c061481-a275-4897-8951-b4f88223b8d4.png)

🚩Let us add a calculation for simulated sales revenue. 

103. Click **More Action** Icon for the **Account Dimension**

104. Click **Add Calculation**

![8-78](https://user-images.githubusercontent.com/92877810/141008243-35608fb8-b076-4df5-871b-0950315d87f6.png)

105. Click **Calculated Measure**

![8-79](https://user-images.githubusercontent.com/92877810/141008244-09e5e925-afce-40fa-8c7c-eef44929cdcd.png)

106. Rename the Calculation to **Simulated Sales Revenue**

107. Type **"Sa"**

108. Click **["ANA260_ORDER_FINANCE":Sales_Revenue]** 

![8-80](https://user-images.githubusercontent.com/92877810/141008247-9febb042-45ea-4cee-8cf2-da4246ccaf3a.png)

109. Type in **"*" (Multiplication Sign)**
  
🚩We are using a calculation input control in this calculation. Calculation input controls allow the viewer of the story to adjust the value in the formula through a widget on the page. This interactivity is key to our simulated financial statement

110. Click **+ Create New**

![8-81](https://user-images.githubusercontent.com/92877810/141008249-bf35a515-7052-4e96-9f11-e8d30100a473.png)

🚩Calculation input controls can be created using values in Existing Dimensions or through values defined in a Static List. We want to create a static list of Revenue Multiplier values

111. Click **Revenue Multiplier**

112. Click **Static List**

113. Expand **Values**

![8-82](https://user-images.githubusercontent.com/92877810/141008250-e65ff065-fc7d-4e1b-b842-fb1bdbf3fb5e.png)

🚩Let us define a range of possible values to multiply our simulated sales revenue by. 

114. Click **Select by Range**

![8-83](https://user-images.githubusercontent.com/92877810/141008251-69e389a9-e750-41d2-a13f-1097c14baac2.png)

115. Input **1** as the Min Value

116. Input **2.5** as the Max Value

117. Input **0.1** as the Increment Value

118. Click **OK**

![8-84](https://user-images.githubusercontent.com/92877810/141008252-b0b17ef6-a465-44a4-a60d-ab25e65856f1.png)

119. Click **OK**

![8-85](https://user-images.githubusercontent.com/92877810/141008253-bfabe145-a45b-4dae-a7ae-0ba23566fe64.png)

120. Click **Revenue Multiplier**

121. Click **OK**

![8-86](https://user-images.githubusercontent.com/92877810/141008254-cfd96451-53e5-4167-a732-1a51a7f0bd29.png)

122. Drag our new Input Control to the left of the table (if not already on the left)

![8-87](https://user-images.githubusercontent.com/92877810/141008255-d1645320-85b3-4852-a79d-d33debe77756.png)

🚩Now we can test to see how our Revenue Multiplier input control can help simulate values in our table. 

123. Resize the **Revenue Multiplier Calculation Input Control**

![8-88](https://user-images.githubusercontent.com/92877810/141008258-5bb79042-c518-4d7a-8bc5-456e0a88d32a.png)

⚠️Quality check! Does your revenue multiplier and table look like this screenshot? Let us try simulating some values. 

![8-89](https://user-images.githubusercontent.com/92877810/141008261-b3e1f85b-c50f-4857-9db3-ade42dde07e2.png)

124. Drag the Revenue Multiplier to **1.5**

![8-90](https://user-images.githubusercontent.com/92877810/141008263-8b256ed2-31ad-4c27-a294-f864f90bbd47.png)

⚠️Quality check! Do the values on your table look like this after changing the calculation input control? Using the calculation input control for a simulation improves the interactivity of our dashboard for the use of the story viewer.

![8-91](https://user-images.githubusercontent.com/92877810/141008264-f77e7796-3577-41d6-8470-c0630105d424.png)

⚠️  
Quality check! Does your dashboard look like this screenshot? 

🚩Please save your story by pressing **Ctrl + S** on your keyboard! 
 
ℹ️You have now completed the **Calculations and Blending Jump Off**. In this section we have covered how to create a calculated dimension with string functions, how to link dimensions and use blending for visualizations, how to create calculations with measures across models, how to apply linked analysis between charts with different models, how to use median and quartile aggregations, and how to use calculation input controls to create simulated calculations. 

![8-92](https://user-images.githubusercontent.com/92877810/141008266-c8f2fa21-b252-4f74-9c85-0e080e39f85a.png)

<br><br>

## Summary

**You have completed the entire Time Analysis section!**

**You are now able to:**
- Create calculated dimensions with string functions to enhance your data
- Understand how to blend data models by linking on common dimensions
- Employ statistical calculations in aggregations of your data
- Integrate calculation input controls to simulate values in your visualizations
