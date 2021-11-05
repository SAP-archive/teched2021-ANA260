**Sec 8 will be finished in < 1 hr**

⚠️Does your Dashboard look like this?

1. Click the **Main Menu** icon

![8-1](https://user-images.githubusercontent.com/92877810/140549559-34510e1a-ab16-4d15-8a09-44780b9bbf21.png)

2. Click **Files**

![8-2](https://user-images.githubusercontent.com/92877810/140549561-b6bb2640-ee6a-4e33-aa3a-caf0dcb0268b.png)

3. Click **Public**

![8-3](https://user-images.githubusercontent.com/92877810/140549562-a6349f0f-d727-4dae-920c-fe0b38d245b9.png)

4. Click **TechEd 2021**

![8-4](https://user-images.githubusercontent.com/92877810/140549563-026d102d-db04-4e00-b57a-12fe5e714d6c.png)

5. Select **Section 8.0 - Calculations and Blending (Start)** 

6. Click **Copy** icon

![8-5](https://user-images.githubusercontent.com/92877810/140549565-9a67f98d-96ba-4ce6-84fd-aa5dc77c1e50.png)

🚩Save the file in **MyFiles**

7. Save the file as **"ANA26-_Section 8_Your Initials"**

![8-6](https://user-images.githubusercontent.com/92877810/140549566-fa6f2184-6822-450c-8b7b-65fe99d9a2ce.png)

8. Click **MyFiles**

![8-7](https://user-images.githubusercontent.com/92877810/140549567-953abbcf-397b-4831-ab33-bf72f9ac624b.png)

9. Click **ANA260_Section 8_KG**

![8-8](https://user-images.githubusercontent.com/92877810/140549568-4350e00b-8975-4431-ba21-205a0d5940f0.png)

10. Click **Edit** 

![8-9](https://user-images.githubusercontent.com/92877810/140549570-8cb791c4-e65b-48bd-b300-466a042cd20e.png)

11. Click **Operations Overview**

![8-10](https://user-images.githubusercontent.com/92877810/140549571-579d5608-532b-4339-b6f6-71031341bbad.png)

⚠️Exercise check! Does your dashboard look like this screenshot in Edit mode? 

![8-11](https://user-images.githubusercontent.com/92877810/140549572-32e4b1d1-b581-48c1-9471-0495b26b0d58.png)

🚩When working with your data in SAP Analytics Cloud, you may find that you want to look at additional components to your data that are currently not captured by the existing measures and dimensions in the model. Luckily, story designers can extend the data models with additional calculated measures and dimensions. This enables the story creator to delve into further insights from their data. Let us start by creating a calculated dimension that divides the Store dimension in our data into Studios and Non-Studios. 

12. Click **Gross Margin % for Actual** Chart

![8-12](https://user-images.githubusercontent.com/92877810/140549574-27a28c0e-3bbd-4177-9372-dcbaac4c3f89.png)

13. Click **Designer**

14. Click **+ Add Dimension**

![8-13](https://user-images.githubusercontent.com/92877810/140549575-adc20077-0840-448b-85ba-9ad193b00792.png)

15. Scroll and Click **+ Create Calcluated Dimension...**

![8-14](https://user-images.githubusercontent.com/92877810/140549576-2709a2d4-a0e6-4806-9343-53c95bb32708.png)

ℹ️Welcome to Calculated Dimensions!  
  
Calculated Dimensions are useful when you want to enrich your dimension if your model does not have the needed format. 
 
You can choose to combine existing dimensions to create your own dimensions. There are two calculated dimensions that can be created: 
  
**Calculated Dimension:** Use formulas to create new dimension members 
  
**Measure Based Dimension:** Use ranges within an existing measure to determine how to group 
dimension members together 

![8-15](https://user-images.githubusercontent.com/92877810/140549577-68a72378-205b-4bef-9837-95e0b6cacd81.png)

🚩As we want to identify the stores that are studios, we will use the regular calculated dimension. 

16. Click **Calculated DImension**

![8-16](https://user-images.githubusercontent.com/92877810/140549579-56cd9530-2c68-4d46-90fb-7e2310dc2b15.png)

🚩The formula field for Calculated Dimensions uses conditional logic and function formulas to create the Dimension rules. This offers the business analyst great flexibility in defining new calculated dimensions. 

17. Press **Ctrl + Space** on the Keyboard

![8-17](https://user-images.githubusercontent.com/92877810/140549580-b8f0fe2d-d25b-454b-b294-295375e2cbf3.png)

18. Click IF

🚩Our IF statement has three fields. The first field is used as a condition that evaluates to true or false. The second field is the Dimension value if True and the third field is the Dimension value if False. 

![8-18](https://user-images.githubusercontent.com/92877810/140549582-9615bda3-5c9e-48f8-80ed-91b9566353fe.png)

19. Click the **Condition (First Field)** in the IF Formula

![8-19](https://user-images.githubusercontent.com/92877810/140549585-5cd5024c-5dc0-465d-9395-f3870ccd5518.png)

20. Press **Ctrl + Space** on the Keyboard
  
💡Using Ctrl + Space is a great way to learn how to use the Calculation Editor. Using this hotkey combination will always bring up all possible functions and measures/dimensions that can be typed into the according field for the ease of the user. 

![8-20](https://user-images.githubusercontent.com/92877810/140549586-a9e20b48-650a-473c-8589-37f5080612cc.png)

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

![8-21](https://user-images.githubusercontent.com/92877810/140549589-fe998e0a-ab3b-4b17-a176-05b03259f06b.png)

🚩Here we are specifying the Dimension we are reading our string from

23. Type **St** in the **First Input Field** for **RIGHT**

24. Click **Store**

![8-22](https://user-images.githubusercontent.com/92877810/140549591-334bb3da-91df-458e-b4aa-55e2a2388144.png)

ℹ️Since Dimensions often have an ID and 
Description, it is important to clarify that we are looking to parse the Store name from description here. 

25. Type in a **Period "."**

26. Press **Ctrl + Space** on the keyboard

27. Click **Description**

![8-23](https://user-images.githubusercontent.com/92877810/140549593-70ae4a45-9d0c-4a2d-b0f2-ec799fd55f00.png)

🚩We know we are trying to divide our Store dimension into Studios and Non-Studio. Since we are looking for "Studio" at the end of store name, we know we should filter on 6 characters using our RIGHT string function. 

28. Type **"6"** in the **Second Input Field** for the **RIGHT** Function

![8-24](https://user-images.githubusercontent.com/92877810/140549594-21b9d667-0d1b-458b-8cbd-2617a5b6c9e9.png)

🚩Let us compare the last 6 letters of our store name with Studio to group them into two Store Groups. 

29. Type in =**"Studio"** following the RIGHT formula

30. Type in **"Studio"** in the **TRUE** Field for the IF Function

31. Type in **"Non-Studio"** in the **FALSE** Field for the  IF Function

![8-25](https://user-images.githubusercontent.com/92877810/140549595-59e377a7-7be1-4add-8a3e-0ab1a4c67ccb.png)

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

48. Click **Link Attribute**

49. Click **Description**

![8-39](https://user-images.githubusercontent.com/92877810/140554047-cb7439d2-a9b8-45ec-92f0-2926976d790d.png)

50. Click **Link Attribute**

51. Click **Description**

52. Click **Set**

![8-40](https://user-images.githubusercontent.com/92877810/140554048-587bd199-3237-40ab-8a79-fd6c599d842e.png)

🚩SAP Analytics Cloud will display the model links you have created to link dimensions. We could choose to edit these links or add more linked dimensions. 

53. Click **Done**

![8-41](https://user-images.githubusercontent.com/92877810/140554051-7448a98d-e2de-46c8-a40e-ceea581d032e.png)

🚩Now that we have Linked Dimensions, we can create blended visualizations to look at correlations in our data. As a business analyst, we may be concerned about shipping delays and how it affects our company revenue. Let us look at a blended table to display information that would help this analysis

54. Scroll to the Right of the Dashboard

55. Click **ANA260_Shipping_Info** Table

![8-42](https://user-images.githubusercontent.com/92877810/140554053-4b750b64-2b8b-4bf3-ad27-8be37cafe3ee.png)

56. Click **+ Add Linked Models**

![8-43](https://user-images.githubusercontent.com/92877810/140554054-68697cb0-bef5-4621-bd00-c103dd801dd1.png)

57. Click **ANA260_ORDER_FINANCE**

ℹ️We are now able to see ANA260_ORDER_FINANCE as a linkable model to this table because we have linked it to our Shipping model on Order Number and Store dimensions. 
  
We can choose to display measures and calculations across our columns from both models to look at the relationships in the data. 
  
In this table, we have specified Reasons for Delay as our Row dimension. We can look at how our Finance data is affected in each of these delay members. 

![8-44](https://user-images.githubusercontent.com/92877810/140554055-d4ed9d76-5abc-461b-a0af-5590964e5dff.png)

🚩Let us create a calculation using Finance data to see how much of our product revenue falls under each of the Reasons for Delay categories. 

58. Click the **More Action** Icon for the **Account Dimension**

59. Click **Add Calculation**

60. Click **ANA260_ORDER_FINANCE**

![8-45](https://user-images.githubusercontent.com/92877810/140554057-7652be75-e3ab-4e66-ad5e-eaa8f727fade.png)

61. Rename the Calculation to % **Contribution to Revenue**

![8-46](https://user-images.githubusercontent.com/92877810/140554058-c7b4d44e-bc93-4b10-95eb-eac572812d2b.png)

62. Type in "%" in Edit Formula

63. Select **%GrandTotal**

![8-47](https://user-images.githubusercontent.com/92877810/140554060-a621a52e-31f0-497d-83b7-3d70bf80a437.png)

64. Type in **"Re"** in %GrandTotal Field

65. Click **["ANA260_ORDER_FINANCE":Sales_Revenue]** 

66. Click **OK**

![8-48](https://user-images.githubusercontent.com/92877810/140554061-40e1fc37-da1c-42dd-b541-a252c7416797.png)

🚩Our table has updated with this calculation, but it has also included many other measures from the Finance model. First, we need to filter what columns are included in the table. 

67. Click **Filter**

68. Click **ANA260_ORDER_FINANCE**

![8-49](https://user-images.githubusercontent.com/92877810/140554062-e9fd33d2-a946-47f1-8d5f-576948a9837d.png)

69. Scroll and Click **% Contribution to Revenue**

70. Click **OK**

![8-50](https://user-images.githubusercontent.com/92877810/140554064-9b63ef6a-b6e2-484c-967a-0e0237fe7bb9.png)

⚠️Quality Check! Does your table look like this screenshot? 

🚩We can see how useful blended visualizations can be with multiple data sets. From this table, we can see that around 42% of our revenue ships on time. However, weather conditions and out of stock also have relatively high % contributions to revenue. We should probably consider inventory management improvements as over 11% of our revenue in shipments are delayed due to being Out of Stock. 

![8-51](https://user-images.githubusercontent.com/92877810/140554065-cea38047-1403-494a-974b-53ca2ff750db.png)

🚩We can create calculations with measures from both models for visualization purposes. Let us look at the relationship between average order size from our stores and the delivery time

71. Scroll down 

72. Click the **Store Order Size per Store for Actual** Chart

![8-52](https://user-images.githubusercontent.com/92877810/140554067-20718442-2f86-4ee8-8404-52e63cd19e32.png)

🚩Once again, our visualization has a linked model for Finance. Let us add a new measure for Store Order Size. 

73. Click **Add Measure** 

![8-53](https://user-images.githubusercontent.com/92877810/140554068-71c9e198-a08f-4c5e-8fba-666badb21014.png)

74. Click **ANA260_SHIPPING_INFO**

![8-54](https://user-images.githubusercontent.com/92877810/140554069-9903484e-4b61-40cf-8b9c-4b6cd49d2f48.png)

75. Click **Store Order Size**

76. Click Inside the Builder Panel to collapse the Measure Selection drop - down menu 
 
![8-55](https://user-images.githubusercontent.com/92877810/140554070-fef8cd4c-554a-4d0c-a3f9-d867f2a80daf.png)

⚠️Quality check! Does your chart appear like this screenshot? 
 
**Note:** You might have a different color chart

![8-56](https://user-images.githubusercontent.com/92877810/140554071-feada96e-c27f-463b-9c7c-0f614fa64447.png)

ℹ️Let us look at how this calculation was created. We can easily examine the formula by going into the options

77. Click **More Action** Icon for **Store Order Size**

78. Click **Edit Calculation**

![8-57](https://user-images.githubusercontent.com/92877810/140554073-bb572f64-9069-4682-a934-f0c0163229a3.png)

🚩Here is the formula for Store Order Size. It is a calculation using Sales Revenue from the Finance model and a Count 
Aggregation from the Shipping Model for the Number of Delivered Orders. Since we are blending on Store name, our chart will understand this context for our Shipping aggregation. 

79. Click **OK**

![8-58](https://user-images.githubusercontent.com/92877810/140554075-629191d6-14b6-4e8b-a4e4-55c85a2d7a78.png)

🚩Let us use a Top N ranking to sort our chart data since we are interested in analyzing our top performing stores rather than all our stores. 

80. Click **More Actions**

81. Click **Rank**

82. Click **Top N Options**

![8-59](https://user-images.githubusercontent.com/92877810/140554077-6d7777df-3207-45f6-b67c-7d3ed60ed0cc.png)

83. Set Value to 10

84. Click **Apply**

![8-60](https://user-images.githubusercontent.com/92877810/140554078-1393f924-ff32-430d-95c8-00de10be16cb.png)
