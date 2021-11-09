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

![8-1](https://user-images.githubusercontent.com/92877810/141001191-4f0c4613-5aa2-48d4-9d66-142a4e976eee.png)

2. Click **Files**

![8-2](https://user-images.githubusercontent.com/92877810/141001193-c202d0f4-690b-4593-9128-5c93cf601625.png)

3. Click **Public**

![8-3](https://user-images.githubusercontent.com/92877810/141001195-893057f1-b4f4-4265-a71a-70358d57f840.png)

4. Click **TechEd 2021**

![8-4](https://user-images.githubusercontent.com/92877810/141001196-634601bd-3dab-4bc4-94a4-2f231eb4cfa8.png)

5. Select **Section 8.0 - Calculations and Blending (Start)** 

6. Click **Copy** icon

![8-5](https://user-images.githubusercontent.com/92877810/141001198-38ff6f03-a106-447b-af34-e9418a817735.png)

🚩Save the file in **MyFiles**

7. Save the file as **"ANA26-_Section 8_Your Initials"**

![8-6](https://user-images.githubusercontent.com/92877810/141001200-e232eddb-227d-4b3e-bd92-16568579f20e.png)

8. Click **MyFiles**

![8-7](https://user-images.githubusercontent.com/92877810/141001201-cc255abe-cabf-494c-a1cc-2d3228ad09aa.png)

9. Click **ANA260_Section 8_KG**

![8-8](https://user-images.githubusercontent.com/92877810/141001203-e9c2bb70-4c95-4aa0-897a-01c296738941.png)

10. Click **Edit** 

![8-9](https://user-images.githubusercontent.com/92877810/141001204-dfcaa281-09b9-4786-b58c-98a177a2c46e.png)

11. Click **Operations Overview**

![8-10](https://user-images.githubusercontent.com/92877810/141001206-54cf13a0-6b64-4f20-a6e9-d0c6a666364d.png)

⚠️Exercise check! Does your dashboard look like this screenshot in Edit mode? 

![8-11](https://user-images.githubusercontent.com/92877810/141001207-38cb21c3-afcc-4afe-97e3-2654decbcd5e.png)

🚩When working with your data in SAP Analytics Cloud, you may find that you want to look at additional components to your data that are currently not captured by the existing measures and dimensions in the model. Luckily, story designers can extend the data models with additional calculated measures and dimensions. This enables the story creator to delve into further insights from their data. Let us start by creating a calculated dimension that divides the Store dimension in our data into Studios and Non-Studios. 

12. Click **Gross Margin % for Actual** Chart

![8-12](https://user-images.githubusercontent.com/92877810/141001210-6972c75e-d8e4-41d5-8277-e6a0f1f125b5.png)

13. Click **Designer**

14. Click **+ Add Dimension**

![8-13](https://user-images.githubusercontent.com/92877810/141001213-4780958e-36a7-48ba-80d4-fd2dae6fcfc7.png)

15. Scroll and Click **+ Create Calcluated Dimension...**

![8-14](https://user-images.githubusercontent.com/92877810/141001215-0c23dda2-e371-4ea9-b899-98402a7555bd.png)

ℹ️Welcome to Calculated Dimensions!  
  
Calculated Dimensions are useful when you want to enrich your dimension if your model does not have the needed format. 
 
You can choose to combine existing dimensions to create your own dimensions. There are two calculated dimensions that can be created: 
  
**Calculated Dimension:** Use formulas to create new dimension members 
  
**Measure Based Dimension:** Use ranges within an existing measure to determine how to group 
dimension members together 

![8-15](https://user-images.githubusercontent.com/92877810/141001216-206f391e-838f-4990-bfa6-a4c54f412bde.png)

🚩As we want to identify the stores that are studios, we will use the regular calculated dimension. 

16. Click **Calculated DImension**

![8-16](https://user-images.githubusercontent.com/92877810/141001218-95abc1d1-e88a-4f5e-86e6-0297cd012253.png)


🚩The formula field for Calculated Dimensions uses conditional logic and function formulas to create the Dimension rules. This offers the business analyst great flexibility in defining new calculated dimensions. 

17. Press **Ctrl + Space** on the Keyboard

![8-17](https://user-images.githubusercontent.com/92877810/141001219-fafdb6a7-630b-4794-a941-949be5bad762.png)

18. Click IF

🚩Our IF statement has three fields. The first field is used as a condition that evaluates to true or false. The second field is the Dimension value if True and the third field is the Dimension value if False. 

![8-18](https://user-images.githubusercontent.com/92877810/141001220-064fbdca-e32b-4ac0-bc57-a128c43dbd54.png)

19. Click the **Condition (First Field)** in the IF Formula

![8-19](https://user-images.githubusercontent.com/92877810/141001222-7e10a669-1844-4cc1-ba71-2d2cfeff1abb.png)

20. Press **Ctrl + Space** on the Keyboard
  
💡Using Ctrl + Space is a great way to learn how to use the Calculation Editor. Using this hotkey combination will always bring up all possible functions and measures/dimensions that can be typed into the according field for the ease of the user. 

![8-20](https://user-images.githubusercontent.com/92877810/141001223-3c34b82b-ad11-411c-a0e4-7e17a3ff1605.png)

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

21. Scroll till **RIGHT** is **Visible**

22. Click **RIGHT**

![8-21](https://user-images.githubusercontent.com/92877810/141001226-0d25fc27-6b0e-4f29-acf4-bff8ab0ac983.png)

🚩Here we are specifying the Dimension we are reading our string from

23. Type **St** in the **First Input Field** for **RIGHT**

24. Click **Store**

![8-22](https://user-images.githubusercontent.com/92877810/141001227-22d4256f-12d5-465c-81c6-5d8e36f51fa7.png)

ℹ️Since Dimensions often have an ID and 
Description, it is important to clarify that we are looking to parse the Store name from description here. 

25. Type in a **Period "."**

26. Press **Ctrl + Space** on the keyboard

27. Click **Description**

![8-23](https://user-images.githubusercontent.com/92877810/141001228-d237c7fa-3597-42d9-bdb5-dd169025b3e1.png)

🚩We know we are trying to divide our Store dimension into Studios and Non-Studio. Since we are looking for "Studio" at the end of store name, we know we should filter on 6 characters using our RIGHT string function. 

28. Type **"6"** in the **Second Input Field** for the **RIGHT** Function

![8-24](https://user-images.githubusercontent.com/92877810/141001229-fca4ebcc-f2fa-48f2-b79f-7a0d2837160d.png)

🚩Let us compare the last 6 letters of our store name with Studio to group them into two Store Groups. 

29. Type in =**"Studio"** following the RIGHT formula

30. Type in **"Studio"** in the **TRUE** Field for the IF Function

31. Type in **"Non-Studio"** in the **FALSE** Field for the  IF Function

![8-25](https://user-images.githubusercontent.com/92877810/141001230-457d5b2a-8277-4f94-8222-7d2b1d4a3492.png)

⚠️Quality Check! Does the end of your formula look like this? 

![8-26](https://user-images.githubusercontent.com/92877810/140549596-a6b917c3-b702-49e0-ba9a-1f401a72fd41.png)

🚩Format will parse your Formula and identify if there are any problems with the input parameters. 

32. Click **Format** to Validate the Formula
  
🚩Great! Our formula is valid and good for use in defining a new Calculated Dimension. Let us name this Dimension and use it in our charts. 

![8-27](https://user-images.githubusercontent.com/92877810/140549597-31e851c6-c35b-4536-9523-107b69e54e04.png)

33. Name the Calculated Dimension as **Store Group**

34. Click **OK**

![8-28](https://user-images.githubusercontent.com/92877810/140549599-466141d1-921b-4d59-a929-c4a8b6a0c12a.png)

⚠️Quality check! Does your chart look like this after including your Calculated Dimension? 

🚩By creating a Calculated Dimension, we are able extract further insights from our data. We can now see that Gross Margin % is higher for Studios than other stores. This could be of interest to us for further financial analysis and investments. 

![8-29](https://user-images.githubusercontent.com/92877810/140549600-0b8c5372-3354-417b-acfa-1dbe46a1e743.png)

🚩Let us use our new Calculated Dimension to find out the split of Average Sales Revenue by Store Group. 

35. Click Avg Sales Revenue for Actual Chart

![8-30](https://user-images.githubusercontent.com/92877810/140549603-8c0a65f3-0e30-4d04-8242-f36a6cef9d1f.png)

36. Click **+ Add Dimension** 

![8-31](https://user-images.githubusercontent.com/92877810/140554035-5d406625-989b-4baa-95f4-39c69a528e07.png)

37. Scroll and Click **Store Group**

38. Click Inside the Builder Panel to Collapse the Dimension Selection Drop Down Menu 

![8-32](https://user-images.githubusercontent.com/92877810/140554037-ab975a17-23ff-4641-b8e5-270b2d6f1ad6.png)

⚠️Quality check! Do your charts look like this screenshot? 
  
🚩We can now see that Avg Sales Revenue is also higher for Studio Stores. It could be a good business decision to change our contract structure with our Studio Stores! 

![8-33](https://user-images.githubusercontent.com/92877810/140554039-db560268-4991-414b-b69f-9589b723809f.png)

🚩Up until this point, we have been working with visualizations built from measures and dimensions spanning a single model. Now, we can improve the value of our analysis through Blending to combine data sources. We can accomplish this by linking dimensions across models so we can compare and analyze the relationship between measures and dimensions across multiple models

ℹ️If you are missing the icon for Link Dimensions in your toolbar, click on 
... under More to surface this option. 

39. Click **Link Dimensions**

![8-34](https://user-images.githubusercontent.com/92877810/140554041-9111d980-223d-480f-954c-3d27ca9709ab.png)

ℹ️Welcome to Link Dimensions! 
  
Link Dimensions allow you to create blended visualizations that display data from multiple models. It also allows you to create filters that simultaneously update all visualization that include linked data regardless of the model.  
  
By default, the ID attribute is used to match members between the linked dimensions. However, for non-hierarchy dimensions it is possible to change the description that is used for linking. 

We can utilize Linked Dimensions in our data by linking across the Finance and Shipping models by connecting dimensions that are identical across our two models. 

![8-35](https://user-images.githubusercontent.com/92877810/140554043-d42dfb93-1be3-4934-bca9-4d47c2ac8b51.png)

🚩Let us link the Order Number and Store dimensions between our two models. Both these dimensions are identical across our models and have independent members that we can gather insights from. By linking on Store and Order Number we can look at analyses that target Store entities or individual orders. 

40. Scroll and Click **Order Number**
 
41. Scroll and Click **Order Number**
 
![8-36](https://user-images.githubusercontent.com/92877810/140554044-0149768f-1514-46d0-b447-d97c6f8f9dc3.png)

42. Scroll and Click **Store** 
 
43. Scroll and Click **Store**
 
![8-37](https://user-images.githubusercontent.com/92877810/140554045-0c508e60-5778-4a78-87d5-389c70d87788.png)

🚩It is important to specify the Dimension Attribute we are linking across. Order Number in our models is common on the Dimension ID whereas Store is common on the Dimension Description (the store name). Let us make sure that Order Number is linked by IDs between the models and Store is linked by Description or Store Names between the models. 

44. Click **Link Attribute**

45. Click **ID**

![8-38](https://user-images.githubusercontent.com/92877810/140554046-0e7dc1de-088e-477c-951a-0cf357ede842.png)

46. Click **Link Attribute**

47. Click **ID**

![8-39](https://user-images.githubusercontent.com/92877810/140554047-cb7439d2-a9b8-45ec-92f0-2926976d790d.png)

48. Click **Link Attribute**

49. Click **Description**

![8-40](https://user-images.githubusercontent.com/92877810/140554048-587bd199-3237-40ab-8a79-fd6c599d842e.png)

50. Click **Link Attribute**

51. Click **Description**

52. Click **Set**

![8-41](https://user-images.githubusercontent.com/92877810/140554051-7448a98d-e2de-46c8-a40e-ceea581d032e.png)

🚩SAP Analytics Cloud will display the model links you have created to link dimensions. We could choose to edit these links or add more linked dimensions. 

53. Click **Done**

![8-42](https://user-images.githubusercontent.com/92877810/140554053-4b750b64-2b8b-4bf3-ad27-8be37cafe3ee.png)

🚩Now that we have Linked Dimensions, we can create blended visualizations to look at correlations in our data. As a business analyst, we may be concerned about shipping delays and how it affects our company revenue. Let us look at a blended table to display information that would help this analysis

54. Scroll to the Right of the Dashboard

55. Click **ANA260_Shipping_Info** Table

![8-43](https://user-images.githubusercontent.com/92877810/140554054-68697cb0-bef5-4621-bd00-c103dd801dd1.png)

56. Click **+ Add Linked Models**

![8-44](https://user-images.githubusercontent.com/92877810/140554055-d4ed9d76-5abc-461b-a0af-5590964e5dff.png)

57. Click **ANA260_ORDER_FINANCE**

ℹ️We are now able to see ANA260_ORDER_FINANCE as a linkable model to this table because we have linked it to our Shipping model on Order Number and Store dimensions. 
  
We can choose to display measures and calculations across our columns from both models to look at the relationships in the data. 
  
In this table, we have specified Reasons for Delay as our Row dimension. We can look at how our Finance data is affected in each of these delay members. 

![8-45](https://user-images.githubusercontent.com/92877810/140554057-7652be75-e3ab-4e66-ad5e-eaa8f727fade.png)

🚩Let us create a calculation using Finance data to see how much of our product revenue falls under each of the Reasons for Delay categories. 

58. Click the **More Action** Icon for the **Account Dimension**

59. Click **Add Calculation**

60. Click **ANA260_ORDER_FINANCE**

![8-46](https://user-images.githubusercontent.com/92877810/140554058-c7b4d44e-bc93-4b10-95eb-eac572812d2b.png)

61. Rename the Calculation to % **Contribution to Revenue**

![8-47](https://user-images.githubusercontent.com/92877810/140554060-a621a52e-31f0-497d-83b7-3d70bf80a437.png)

62. Type in "%" in Edit Formula

63. Select **%GrandTotal**

![8-48](https://user-images.githubusercontent.com/92877810/140554061-40e1fc37-da1c-42dd-b541-a252c7416797.png)

64. Type in **"Re"** in %GrandTotal Field

65. Click **["ANA260_ORDER_FINANCE":Sales_Revenue]** 

66. Click **OK**

![8-49](https://user-images.githubusercontent.com/92877810/140554062-e9fd33d2-a946-47f1-8d5f-576948a9837d.png)

🚩Our table has updated with this calculation, but it has also included many other measures from the Finance model. First, we need to filter what columns are included in the table. 

67. Click **Filter**

68. Click **ANA260_ORDER_FINANCE**

![8-50](https://user-images.githubusercontent.com/92877810/140554064-9b63ef6a-b6e2-484c-967a-0e0237fe7bb9.png)

69. Scroll and Click **% Contribution to Revenue**

70. Click **OK**

![8-51](https://user-images.githubusercontent.com/92877810/140554065-cea38047-1403-494a-974b-53ca2ff750db.png)

⚠️Quality Check! Does your table look like this screenshot? 

🚩We can see how useful blended visualizations can be with multiple data sets. From this table, we can see that around 42% of our revenue ships on time. However, weather conditions and out of stock also have relatively high % contributions to revenue. We should probably consider inventory management improvements as over 11% of our revenue in shipments are delayed due to being Out of Stock. 

![8-52](https://user-images.githubusercontent.com/92877810/140554067-20718442-2f86-4ee8-8404-52e63cd19e32.png)

🚩We can create calculations with measures from both models for visualization purposes. Let us look at the relationship between average order size from our stores and the delivery time

71. Scroll down 

72. Click the **Store Order Size per Store for Actual** Chart

![8-53](https://user-images.githubusercontent.com/92877810/140554068-71c9e198-a08f-4c5e-8fba-666badb21014.png)

🚩Once again, our visualization has a linked model for Finance. Let us add a new measure for Store Order Size. 

73. Click **Add Measure** 

![8-54](https://user-images.githubusercontent.com/92877810/140554069-9903484e-4b61-40cf-8b9c-4b6cd49d2f48.png)

74. Click **ANA260_SHIPPING_INFO**
 
![8-55](https://user-images.githubusercontent.com/92877810/140554070-fef8cd4c-554a-4d0c-a3f9-d867f2a80daf.png)

75. Click **Store Order Size**

76. Click Inside the Builder Panel to collapse the Measure Selection drop - down menu 

![8-56](https://user-images.githubusercontent.com/92877810/140554071-feada96e-c27f-463b-9c7c-0f614fa64447.png)

⚠️Quality check! Does your chart appear like this screenshot? 
 
**Note:** You might have a different color chart

![8-57](https://user-images.githubusercontent.com/92877810/140554073-bb572f64-9069-4682-a934-f0c0163229a3.png)

ℹ️Let us look at how this calculation was created. We can easily examine the formula by going into the options

77. Click **More Action** Icon for **Store Order Size**

78. Click **Edit Calculation**

![8-58](https://user-images.githubusercontent.com/92877810/140554075-629191d6-14b6-4e8b-a4e4-55c85a2d7a78.png)

🚩Here is the formula for Store Order Size. It is a calculation using Sales Revenue from the Finance model and a Count 
Aggregation from the Shipping Model for the Number of Delivered Orders. Since we are blending on Store name, our chart will understand this context for our Shipping aggregation. 

79. Click **OK**

![8-59](https://user-images.githubusercontent.com/92877810/140554077-6d7777df-3207-45f6-b67c-7d3ed60ed0cc.png)

🚩Let us use a Top N ranking to sort our chart data since we are interested in analyzing our top performing stores rather than all our stores. 

80. Click **More Actions**

81. Click **Rank**

82. Click **Top N Options**

![8-60](https://user-images.githubusercontent.com/92877810/140554078-1393f924-ff32-430d-95c8-00de10be16cb.png)

83. Set Value to 10

84. Click **Apply**

![8-61](https://user-images.githubusercontent.com/92877810/140558791-07496d08-dcb9-4a10-8a25-d11973dce90a.png)

⚠️Quality check! Does your chart look like this screenshot? 

![8-62](https://user-images.githubusercontent.com/92877810/140558794-566bb5f2-3d86-4da0-b1da-4c4627c15751.png)

🚩We want to use this chart to drive our analysis to be able to filter on a top performing store. Let us use Linked Analysis from this chart to filter other visualizations. 

85. Click **More Actions**

86. Click **Linked Analysis**

![8-63](https://user-images.githubusercontent.com/92877810/140558797-b43692ea-30fe-4e4b-bcd8-5f57614a0397.png)

🚩We want to select which visualizations are impacted by filtering when we select a top performing store. Let us choose only selected widgets for Linked Analysis. 

87. Click Only **Selected Widgets**

![8-64](https://user-images.githubusercontent.com/92877810/140558798-4b862dcf-7095-40a5-8d8b-2452db9f3496.png)

🚩Let us link our blended chart to a chart that 
only uses the Shipping model. Any selections on our original chart will filter to the secondary chart via Store name. 

88. Scroll and Click **Avg Delivery Time per Store for Actual**

89. Click **Apply** 

![8-65](https://user-images.githubusercontent.com/92877810/140558799-0a082550-8217-4cc8-afdc-ca247f8a2f0e.png)

90. Click the First Three Entries in the Store Order Size per Store Chart

![8-66](https://user-images.githubusercontent.com/92877810/140558801-3bcc9a15-1e7c-4cf4-9b3e-bc91f0a253c1.png)

91. Click **Filter**

![8-67](https://user-images.githubusercontent.com/92877810/140558802-76cee994-46a0-470b-8640-6b6934090cd3.png)

⚠️Quality check! Do your two charts look like this screenshot? 
 
**Note:** You might have a different color for your first chart.
  
🚩It looks as if there is a relationship between larger average order size and a faster average delivery. We have filtered using Linked Analysis from our Finance model with Store Order Size to our Shipping model with Avg Delivery Time based on the linking of dimensions we have created previously. 
  
Let us now look a scatterplot to see if Average Delivery Time is affecting our Gross Margin. 

![8-68](https://user-images.githubusercontent.com/92877810/140558803-6dd43a4e-5db0-4326-8169-0a9bd7000575.png)

92. Scroll to the right of the dashboard

93. Click **Avg Delivery Time. Gross Margin per Store for Actual Chart**

![8-69](https://user-images.githubusercontent.com/92877810/140558804-1025ad90-de0e-487c-b01c-ce11c1ba9a4a.png)

🚩Scatterplots are a great way to look at the correlation between two measures in our blended data. We will be comparing the average delivery time and gross margin for each store. Let us move to the Builder panel. 

94. Click **Add Measure**

![8-70](https://user-images.githubusercontent.com/92877810/140558806-5ad94b74-8dd3-42c2-8b26-4248ac4b5f02.png)

95. Click **ANA260_SHIPPING_INFO**

![8-71](https://user-images.githubusercontent.com/92877810/140558807-cb390ec0-1d17-45af-b5c1-bec37bc86cc8.png)

96. Click **Avg Delivery Time**

![8-72](https://user-images.githubusercontent.com/92877810/140558809-6147d9ea-5c26-4852-bcde-58625979b651.png)

97. Click **Add Measure**

![8-73](https://user-images.githubusercontent.com/92877810/140558810-2fcabcc8-0787-4327-8f27-63d5a83b0c0c.png)

98. Click **ANA260_ORDER_FINANCE**

![8-74](https://user-images.githubusercontent.com/92877810/140558812-a364467f-cc69-4147-9154-0133b54a84dd.png)

99. Click **Gross Margin**

![8-75](https://user-images.githubusercontent.com/92877810/140558813-509ffb36-86cf-4787-888d-052c2ba58ca3.png)

⚠️Quality check! Does your scatterplot look like this screenshot? We can see that stores with higher avg delivery time seem to also have lower gross margin

![8-76](https://user-images.githubusercontent.com/92877810/140558815-13349c86-b64c-40b6-8452-a65419e204f0.png)

🚩Let us now test out Calculation Input Controls and simulating values. Here we have a basic financial statement of gross margin, sales revenue, and cost of goods sold calculated by the difference between sales revenue and gross margin. We want to simulate what our gross margin % on each product would be given a simulated sales revenue increase

100. Scroll to the bottom of the Dashboard

101. Click the **ANA260_ORDER_FINANCE** Table

![8-77](https://user-images.githubusercontent.com/92877810/140558816-eb980967-f020-4f2e-b709-01a844067dd0.png)

🚩Let us add a calculation for simulated sales revenue. 

102. Click **More Action** Icon for the **Account Dimension**

103. Click **Add Calculation**

![8-78](https://user-images.githubusercontent.com/92877810/140558817-fb904fee-a62f-42c3-8f7f-3b2b2d0d19f8.png)

104. Click **Calculated Measure**

![8-79](https://user-images.githubusercontent.com/92877810/140558819-97a186e2-97d7-4a76-9146-53ef071e9563.png)

105. Rename the Calculation to **Simulated Sales Revenue**

106. Click **["ANA260_ORDER_FINANCE":Sales_Revenue]** 

![8-80](https://user-images.githubusercontent.com/92877810/140558820-7cb8b4c2-5340-4085-a7e8-f2a995f657fb.png)

107. Type in **"*" (Multiplication Sign)**
  
🚩We are using a calculation input control in this calculation. Calculation input controls allow the viewer of the story to adjust the value in the formula through a widget on the page. This interactivity is key to our simulated financial statement

108. Click **+ Create New**

![8-81](https://user-images.githubusercontent.com/92877810/140558822-6b88f84e-b9c4-4af2-b8d9-3a90dd3b64b6.png)

🚩Calculation input controls can be created using values in Existing Dimensions or through values defined in a Static List. We want to create a static list of Revenue Multiplier values

109. Click **Revenue Multiplier**

110. Click **Static List**

111. Expand **Values**

![8-82](https://user-images.githubusercontent.com/92877810/140558825-02eedf0d-a6dd-450d-9026-935644a78096.png)

🚩Let us define a range of possible values to multiply our simulated sales revenue by. 

112. Click **Select by Range**

![8-83](https://user-images.githubusercontent.com/92877810/140558826-e70db0be-cfb7-40cb-8f54-fa4e00021186.png)

113. Input **1** as the Min Value

114. Input **2.5** as the Max Value

115. Input **0.1** as the Increment Value

116. Click **OK**

![8-84](https://user-images.githubusercontent.com/92877810/140558828-0a5bb909-cf4b-4dae-85f3-061633da0ba5.png)

117. Click **OK**

![8-85](https://user-images.githubusercontent.com/92877810/140558831-09f94829-3dc1-462b-821d-1f85de99bd7e.png)

118. Click **Revenue Multiplier**

119. Click **OK**

![8-86](https://user-images.githubusercontent.com/92877810/140558832-20b61a46-f813-49ad-8380-32e610392f65.png)

120. Drag our new Input Control to the left of the table

![8-87](https://user-images.githubusercontent.com/92877810/140558833-f939b7b7-d2eb-4d7f-b69e-efc687d0522c.png)

🚩Now we can test to see how our Revenue Multiplier input control can help simulate values in our table. 

121. Resize the **Revenue Multiplier Calculation Input Control**

![8-88](https://user-images.githubusercontent.com/92877810/140558834-bfd39519-6f44-4d8b-a464-0fdc635e65a7.png)

⚠️Quality check! Does your revenue multiplier and table look like this screenshot? Let us try simulating some values. 

![8-89](https://user-images.githubusercontent.com/92877810/140558836-8853c122-209d-48f2-97a7-079ed82d38d9.png)

122. Drag the Revenue Multiplier to **1.5**

![8-90](https://user-images.githubusercontent.com/92877810/140558837-e13d2434-a17b-4ea7-bf95-2058140080a4.png)

⚠️Quality check! Do the values on your table look like this after changing the calculation input control? Using the calculation input control for a simulation improves the interactivity of our dashboard for the use of the story viewer.

![8-91](https://user-images.githubusercontent.com/92877810/140558838-c4401c27-cb35-4742-ae51-00677e40ff1c.png)

⚠️  
Quality check! Does your dashboard look like this screenshot? 

🚩Please save your story by pressing **Ctrl + S** on your keyboard! 
 
ℹ️You have now completed the **Calculations and Blending Jump Off**. In this section we have covered how to create a calculated dimension with string functions, how to link dimensions and use blending for visualizations, how to create calculations with measures across models, how to apply linked analysis between charts with different models, how to use median and quartile aggregations, and how to use calculation input controls to create simulated calculations. 

![8-92](https://user-images.githubusercontent.com/92877810/140558839-1c77e933-1e47-4fcf-b120-d8b59e029881.png)

<br><br>

## Summary

**You have completed the entire Time Analysis section!**

**You are now able to:**
- Create calculated dimensions with string functions to enhance your data
- Understand how to blend data models by linking on common dimensions
- Employ statistical calculations in aggregations of your data
- Integrate calculation input controls to simulate values in your visualizations
