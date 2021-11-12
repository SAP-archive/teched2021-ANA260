# Section 10 - Time Analysis Deep Dive

ℹ️**Objective:** Learn how to effectively analyze your time-based data, how to create time-based filters, 
calculations and visualisations. 

**Estimated Time:** 20 mins

**Exercise Description:** You as a business analyst, need to assess company’s performance this year, 
compare operational and finance KPIs over time and learn how to enhance the dashboard with interactive 
capabilities to ensure company’s managers can further investigate the data.

**Key Features:**
- Create dynamic and fixed date-based story and page filters with multiple ranges
- Learn how to customise “current date” for greater flexibility when analysing time-based data
- Create dynamic calculations such as Year-to-Date (YTD), Previous Year-to-Date (PYTD) and others
- Learn how to define date-based hierarchies in SAC that best suit your needs

⚠️**Disclaimer**
When completing exercises, some data values in the screenshots may not match what you see on your 
screen. This is because the dynamic time filters that were applied at the time the screenshots were taken is 
different from the current system date.

----------------------------------------------------------------------------------------------------------------------------------------

⚠️Quality Check! Does your screen look like this screenshot?

![10-r](https://user-images.githubusercontent.com/92877810/141178734-c3c60a37-6251-4139-85f1-5fdb78e7a9df.png)

1. Click **Home**

![10-2](https://user-images.githubusercontent.com/92877810/140169054-660b51b7-cf37-4624-a96a-b8fecdd1e9b1.png)

ℹ️Welcome to the **Time Analysis Deep Dive**! We will also go into greater detail on the analytic capabilities available to story creators and how you can enhance yourdashboard to analyze trends over time

🚩For this section you will start with an existing story. Let's open the starting story from the file repository

2. Click **Files**

![10-3](https://user-images.githubusercontent.com/92877810/140169056-998daf3d-a77b-49a6-96ca-3d553281438d.png)

3. Click **Public**

![10-4](https://user-images.githubusercontent.com/92877810/140169059-1973488d-6ce4-4293-a479-9f79d4583898.png)

4. Click **TechEd 2021**

![10-5](https://user-images.githubusercontent.com/92877810/140169061-d617c612-6c59-4bdc-97f2-28a2b895b86d.png)

5. Click **Section 10.0 - Time Analysis (START)**

![10-6](https://user-images.githubusercontent.com/92877810/140169062-eb3cb0d0-b5aa-4eb8-a0f5-48db8aad82ae.png)

⚠️Quality Check! Ensure this story was opened. 

![10-7](https://user-images.githubusercontent.com/92877810/140169064-840d89eb-f429-401d-84e4-97ae739adf2c.png)

🚩As you do not have edit rights to this story, use Save As to create your own copy. 

6. Click **File**

7. Click **Save As**

![10-8](https://user-images.githubusercontent.com/92877810/140169067-6b87843a-f03d-4cbf-8de5-19949418aa05.png)

8. Save the file as **"ANA260_Section 10_Your Initials"** in MyFiles

9. Click **OK**

![10-9](https://user-images.githubusercontent.com/92877810/140169069-9ffc1636-ffd3-4ef2-a120-1ca08fc9293d.png)

🚩Wait for the story to be copied

10. Click **Edit**

![10-10](https://user-images.githubusercontent.com/92877810/140169070-ff19afcd-86b6-423c-b47a-7236a59550a9.png)

🚩You want to do the time-based analysis on the **Historical Performance** tab.  

11. Select **Historical Performance** Tab

![10-11](https://user-images.githubusercontent.com/92877810/140169071-a4eb9998-7b6c-4389-a49d-aa7e7f9e3f9c.png)

🚩Right now, there is no time-based filter on the dashboard, you want to narrow down the data to the current month to date. Let's create a story filter using the quick filter option for time. 

12. Click **Add Story Filter** icon

13. Click **Current**

![10-12](https://user-images.githubusercontent.com/92877810/140169074-c985912d-855d-4c0b-ab84-0cae89ac8dea.png)

14. Click **Order Date**

15. Click **Month** under **To Date**

![10-13](https://user-images.githubusercontent.com/92877810/140169076-64e2e4ec-ded6-4cad-b75d-047cab4bd661.png)

🚩You can see a story filter for the current month to date has been created and the entire dashboard has been filtered from start of this month until today.  
 
Note: As this is a dynamic time filter, your data may look different based on today's date. 

![10-14](https://user-images.githubusercontent.com/92877810/140169078-22b66009-38bf-4f49-a942-1fb11649052b.png)

🚩  Currently the current month is determined based on system time. However, you want to provide your story viewers with the ability to determine what the current day is. For this you can add a custom current date input control.  

16. Click **Order Date** Story Filter

17. Click **Edit Filter**

![10-15](https://user-images.githubusercontent.com/92877810/140169080-9ac736f9-c054-4b76-bca0-6118de2ac8b9.png)

🚩While you created the month to date filter via quick options, the dynamic range filter dialog provides a lot of more options. First you want to add the custom current date input control.  

18. Expand **Current Date**

19. Click **+ Create Current Date Input Control**

![10-16](https://user-images.githubusercontent.com/92877810/140169081-9adec147-1fe1-4492-bfe6-91983d1897d9.png)

20. Rename to **Date Selector**

21. Expand **Granularity**

22. Click **Day**

![10-17](https://user-images.githubusercontent.com/92877810/140169083-1d1ba002-8a62-4eee-8d9a-440a9604a8fc.png)

🚩Let's set the default current date to 
October 31st, 2021 as it is the last day of last month. 

23. Expand **Day Granularity**

24. Click **January**

25. Click **October**

![10-18](https://user-images.githubusercontent.com/92877810/140169085-ef6c6165-6f00-4375-9ee0-70f0ad31addd.png)

26. Click **31**

![10-19](https://user-images.githubusercontent.com/92877810/140169086-d51f13f5-73af-45c4-99ae-f854ccafd9ae.png)

27. Click **OK**

![10-20](https://user-images.githubusercontent.com/92877810/140169087-27e1421e-bd23-4c5a-9aa5-b19b13f79db5.png)

🚩Quality Check! Does your Dynamic Time Filter match the screenshot? 
  
Note: Range 1: Current Month may not match due to dynamic time. 

28. Click OK

![10-21](https://user-images.githubusercontent.com/92877810/140178403-2e9cd164-249f-4d77-82b8-abf54a658ad8.png)

🚩You can see the Date Selector input control was added to the story filter bar. In the time series chart, you can see that the data now show October data until October 31st.

![10-22](https://user-images.githubusercontent.com/92877810/140178404-59bade35-8056-434f-b739-a7d92f6cb4be.png)

🚩Let's change the Current Date to December 8th, 2021 and see how the dashboard updates. 

29. Click **Date Selector**

30. Click **October**

![10-23](https://user-images.githubusercontent.com/92877810/140178405-225e8565-0e97-4072-bde6-6653f5949f58.png)

31. Click **Dec**

![10-24](https://user-images.githubusercontent.com/92877810/140178407-5e2abe87-4f15-422b-8bbd-b9ae60babe8f.png)

32. Click **8**

33. Click **Outside** the **Date Selector** to Collapse

![10-25](https://user-images.githubusercontent.com/92877810/140178409-64a2408a-cb77-4631-9798-dfd4b6afe749.png)

🚩You can see, especially in the time series chart, that the dashboard has been updated accordingly. 

![10-26](https://user-images.githubusercontent.com/92877810/140178410-d50c15ad-fc77-4c74-aca7-53c5bab70751.png)

🚩Next, you want to give your story viewers some more time filtering options. Such as Current Year to Date and Previous Year to Date. Of course, all these options shall be based on the Date Selector for the current date. 
  
You can do this by adding additional ranges to the Current Month story filter

34. Click **Order Date**

35. Click **Edit Filter**

![10-27](https://user-images.githubusercontent.com/92877810/140178411-a0101ee8-b439-4d94-81fa-0143a1f12b8f.png)

🚩The first range to add is beginning of the year up to today's date. 

36. Click **+ Add a New Range**

![10-28](https://user-images.githubusercontent.com/92877810/140178415-e19aa01f-59ea-40ad-94df-d3981012e658.png)

37. Click **Include Range up to Current Period**

![10-29](https://user-images.githubusercontent.com/92877810/140178416-74b5baa9-b531-4a01-96e9-9b3e611fb65d.png)

🚩The next range to add is beginning of last year up to today's date last year. This can be done by applying an offset to the range filter

38. Click **+ Add a New Range**

![10-r2](https://user-images.githubusercontent.com/92877810/141179788-23e3145c-dfd4-426a-865c-9641bd7035ca.png)

39. Expand **Range Type**

![10-31](https://user-images.githubusercontent.com/92877810/140178420-4e213258-d67d-4cc9-a183-e4fca5a3cfb0.png)

40. Click **Offset**

![10-32](https://user-images.githubusercontent.com/92877810/140178421-134f740b-7b3d-49d1-9587-34e541b6ab48.png)

41. Enter 1 as the Offset Amount

42. Click **Outside** the **Offset Amount**

43. Enable Include Range up to Offset Period

The last range shall be the last 2 years as well as the current year

44. Click + Add a New Range

![10-33](https://user-images.githubusercontent.com/92877810/140178422-88933b20-a648-46dd-94d3-a157422247ab.png)

45. Enter **Look Back** as **2**

46. Click **Outside** Look Back to Save Entry

🚩You're done with the set up of the 4 time ranges that the story view may choose from. 

47. Click **OK**

![10-34](https://user-images.githubusercontent.com/92877810/140178424-e0b05bc6-7100-4a19-b435-96c2b386fd41.png)

🚩Let's review the ranges created. Switch from Current Month to the Current Year filter. 

48. Click **Current Month**

49. Click the **Second Member**

50. Click  outside to collapse the story filter

![10-r50](https://user-images.githubusercontent.com/92877810/141179790-1797e9b4-d882-46be-823e-b797f5ea8576.png)

🚩You can see on the time series chart that the filter has been applied. Let's extend to view the last 2 years as well as the current year. 

![10-r51](https://user-images.githubusercontent.com/92877810/141179791-7ad856bb-9deb-4cb1-b129-49fbe90b391d.png)

51. Click **Order Date**

52. Click the **Last Member**

53. Click  outside to collapse the story filter

![10-r53](https://user-images.githubusercontent.com/92877810/141179792-f8d3464d-3e88-4275-956b-3cce59521258.png)

🚩Again, you can see on the time series chart that the filter has been applied.  

![10-r54](https://user-images.githubusercontent.com/92877810/141179795-cc7a58d4-ac20-4c6f-a51c-315cbddc8766.png)

🚩Right now, the story filter has still a lot of options such as configuring the time periods to go back to. You can hide this complexity from the story viewer. Let's do that and only expose the effected time range to the story viewers. 

54. Click **Order Date**

55. Click **Settings**

56. Click **Show/Hide**

![10-r56](https://user-images.githubusercontent.com/92877810/141179796-04f48fa1-9748-49a4-a195-79ed33a31e2a.png)

57. Deselect **Look Back**

58. Deselect **Current Period**

59. Deselect **Look Ahead**

60. Deselect **Range Info Icons**

![10-r60](https://user-images.githubusercontent.com/92877810/141179797-1662d859-3490-4585-b3e4-9c217a6ec7a6.png)

🚩You can see that this looks much cleaner. 

![10-r61](https://user-images.githubusercontent.com/92877810/141179798-1f65d17a-4e3d-4206-b11c-40f5fe7d7971.png)

🚩Next you want to add some page input controls to investigate, which orders where ordered and received in a certain time frame. These input controls shall be in the lane with the Order Deliver Analysis table. Let's select the lane and add an input control each for Order and Receive Date

61. Click the **Third Lane (Row)**

![10-42](https://user-images.githubusercontent.com/92877810/140178444-b9125fb6-bd3f-4e09-9b6c-275fd79ae71c.png)

62. Click **More** icon

63. Click **Insert Input Control**

![10-43](https://user-images.githubusercontent.com/92877810/140178447-d32ac7ac-d084-4388-a7d5-62b452dcf4f9.png)

64. Click **Dimensions**

![10-44](https://user-images.githubusercontent.com/92877810/140178448-7c1229da-a320-4773-80b7-48fc3352a4fa.png)

65. Click **Order Date**

66. Click **Filter by Range...**

![10-45](https://user-images.githubusercontent.com/92877810/140178449-1efb40f1-9158-4f5f-b452-0776326c577f.png)

🚩This time the range shall be fixed rather than dynamic

67. Click **Fixed**

🚩You want the range of the order to be from October 1st to October 31st, 2021. 

68. Expand **Granularity**

69. Click **Day**

![10-46](https://user-images.githubusercontent.com/92877810/140178451-483912f8-1f00-4d40-b0e7-e0c65d8bfb7d.png)

70. Expand the **Beginning Date Picker**

71. Click **2019**

![10-47](https://user-images.githubusercontent.com/92877810/140178453-9c9e05e1-cc2a-468a-8d02-0092f31dc74a.png)

72. Click **2021**

![10-48](https://user-images.githubusercontent.com/92877810/140178456-496770d7-6651-4424-9b08-b60287200dc5.png)

73. Click **January**

![10-49](https://user-images.githubusercontent.com/92877810/140178459-28632632-e263-4558-8334-0ee56e9f24e5.png)

74. Click **Oct**

![10-50](https://user-images.githubusercontent.com/92877810/140178461-0d321b0f-ce41-440b-824d-06f9e72d47cb.png)

75. Click **1**

![10-51](https://user-images.githubusercontent.com/92877810/140183499-4bfac11e-4784-418c-8cde-7e487b2ff126.png)

76. Expand the **End Date Picker**

![10-52](https://user-images.githubusercontent.com/92877810/140183500-49f3f8e4-e71d-49ae-beeb-5e6fde8454d2.png)

77. Click **December**

![10-53](https://user-images.githubusercontent.com/92877810/140183504-a63ed33b-b494-45dc-9096-6655e5531ffb.png)

78. Click **Oct**

![10-54](https://user-images.githubusercontent.com/92877810/140183506-f94987f2-521f-4732-9f63-f9ed98e113d4.png)

79. Click **31**

![10-55](https://user-images.githubusercontent.com/92877810/140183508-5641ead2-dc17-48ae-b8bf-31b5fbe5f924.png)

⚠️Quality Check! Does your range match the screenshot (October 1, 2021 - October 31, 2021)? 

80. Click **OK**

![10-56](https://user-images.githubusercontent.com/92877810/140183509-ed3ad0d5-b992-4f6c-a4aa-fb3760542126.png)

🚩The input control was added to the page. 
Let's expand it and put it into the position. 

81. Click and Drag the Input Control to Resize

![10-57](https://user-images.githubusercontent.com/92877810/140183510-fdbf960b-33ff-4c34-83c2-259e34776993.png)

⚠️Quality Check! Your dashboard should look like this. 

![10-58](https://user-images.githubusercontent.com/92877810/140183513-aa2a2b65-2575-4e7b-b33c-60420db25599.png)

🚩Let's create another input control to filter based on the receive dates between October 1st, 2021 and November 30th, 2021. 
 
82. Click the **Third Lane (Row)**

![10-59](https://user-images.githubusercontent.com/92877810/140183516-cc73507a-eb78-4f13-8840-a37febe3ac8c.png)

83. Click **More** icon

84. Click **Insert Input Control**

![10-60](https://user-images.githubusercontent.com/92877810/140183519-8a59437b-5cc2-44f1-8f47-91299e9e24cb.png)

85. Click **Dimensions**

![10-61](https://user-images.githubusercontent.com/92877810/140183520-145ef2af-5690-42c1-aae4-cad903883a7d.png)

86. Scroll and Click **Receive Date**

87. Click **Filter by Range...**

![10-62](https://user-images.githubusercontent.com/92877810/140183521-d4b48d15-4e55-4dc5-b5f4-b312ca5519fb.png)

88. Click **Fixed**

89. Expand **Granularity**

90. Select **Day**

![10-63](https://user-images.githubusercontent.com/92877810/140183523-3320a620-6a3f-4284-b8c8-73958b547b4d.png)

91. Expand the **Beginning Date Picker**

![10-64](https://user-images.githubusercontent.com/92877810/140183524-ac559a22-2620-4db0-af07-a59a9cf85ee1.png)

92. Click **2019**

![10-65](https://user-images.githubusercontent.com/92877810/140183528-f9435537-ccc3-412c-ba03-56986bb641db.png)

93. Click **2021**

![10-66](https://user-images.githubusercontent.com/92877810/140183529-c8546be5-6be2-4b3c-a210-e20b370ab1df.png)

94. Click **January**

![10-67](https://user-images.githubusercontent.com/92877810/140183530-3b8994e3-e4d0-4540-b5e9-75c3365df60d.png)

95. Click **Oct**

![10-68](https://user-images.githubusercontent.com/92877810/140183531-705b282e-f0bf-4569-bee7-3e8d885aaaca.png)

96. Click **1**

![10-69](https://user-images.githubusercontent.com/92877810/140183533-38b8b7d0-f2b6-48d5-a6dd-4f6ae4dff7ad.png)

97. Expand the **End Date Picker**

![10-70](https://user-images.githubusercontent.com/92877810/140183534-2b4270f6-8ae2-48ee-bfe1-7b6d3adaf9c0.png)

98. Click **2022**

![10-71](https://user-images.githubusercontent.com/92877810/140186478-4cc111fd-32e1-412c-bf52-fded6ab542a5.png)

99. Click **2021**

![10-72](https://user-images.githubusercontent.com/92877810/140186481-a8ceac4e-65bc-4891-a16a-62933c4fa814.png)

100. Click **January**

![10-73](https://user-images.githubusercontent.com/92877810/140186484-d3ad7ab3-e1b0-4932-b5fe-dc58f630e829.png)

101. Click **Nov**

![10-74](https://user-images.githubusercontent.com/92877810/140186486-3e52fc92-a5c7-465d-a14d-55748b355a20.png)

102. Click **30**

![10-75](https://user-images.githubusercontent.com/92877810/140186489-8c60ad7f-0e58-443b-bda2-fc5b1cb272ad.png)

⚠️Quality Check! Does your range match the screenshot (October 1, 2021 - November 30, 2021)? 

103. Click **OK**

![10-76](https://user-images.githubusercontent.com/92877810/140186492-b58e50f6-edbc-4b7f-b55c-e39ffd647ead.png)

🚩The input control was added to the page. Let's expand it and put it into the position. 

104. Reszie **Receive Date** as Wide as **Order Date Range Filter**

![10-77](https://user-images.githubusercontent.com/92877810/140186493-fb79cf82-398e-4102-a740-069d7ae9c547.png)

⚠️Quality Check! Your dashboard should look like this. 

![10-78](https://user-images.githubusercontent.com/92877810/140186494-39826280-9dcc-4609-950d-aaf27eb6eca1.png)

🚩You may have noticed that the entire dashboard is filtered on the Order and Receive date input controls that you just added. You only want to apply these to the Order Delivery Analysis table. You can use Linked Analysis to set the scope of the page input controls

105. Click the **Order Date Range Filter**

106. Click the **More Action**

107. Click **Linked Analysis**

![10-80](https://user-images.githubusercontent.com/92877810/141184244-994d348c-b401-4902-ad72-14760e0e9700.png)

108. Click **Only Selected Widgets**

![10-81](https://user-images.githubusercontent.com/92877810/141184246-5eb54781-a6de-4d13-a4d8-5a2ca792d60c.png)

109. Scroll and Click **Order Delivery Analysis**

110. Click **Apply**

![10-82](https://user-images.githubusercontent.com/92877810/141184247-e01aa484-1816-4f2c-bb8b-7633b7efea67.png)

🚩We want to repeat the steps for the 
Receive Date Range Filter Input Control. 

111. Click **Receive Date Range Filter**

112. Click **More Action** icon

113. Click **Linked Analysis**

![10-83](https://user-images.githubusercontent.com/92877810/141184249-09132d0b-0e37-45cf-ae2a-dfe4a65afc9a.png)

114. Click **Only Selected Widgets**

![10-84](https://user-images.githubusercontent.com/92877810/141184250-ac6c00e4-0502-49b1-8bd7-fe4f3591c63e.png)

115. Scroll and Click **Order Delivery Analysis**

116. Click **Apply**

![10-85](https://user-images.githubusercontent.com/92877810/141184251-1ab25407-b841-47c1-a810-907dde6e653f.png)

⚠️Quality Check! Your page input controls should only drive the Order Delivery Analysis table

![10-86](https://user-images.githubusercontent.com/92877810/141184252-3612b49b-afd5-455e-b201-986e8197f61f.png)

🚩Let's find out which orders that were shipped after Oct 1st, 2021 have been received by October 8th, 2021. 

117. Click the **End Date Picker**

![10-87](https://user-images.githubusercontent.com/92877810/141184253-32dca347-697d-451f-be38-128291b79c9e.png)

118. Click **November**

![10-88](https://user-images.githubusercontent.com/92877810/141184254-24b0025d-07ce-4fe7-a80c-9a7049d451ac.png)

119. Click **Oct**

![10-89](https://user-images.githubusercontent.com/92877810/141184255-da68786f-8e7a-439c-b38c-a0e5c8c62516.png)

120. Click **8**

![10-90](https://user-images.githubusercontent.com/92877810/141184257-ed38e2c6-ae45-4b60-9d30-60b78b2d1a82.png)
  
🚩Next you want to calculate the time it takes to deliver your orders. This can easily be done via calculations. 

121. Click the **Order Delivery Analysis Table**

![10-91](https://user-images.githubusercontent.com/92877810/141184258-1015bbd5-e08a-441f-b3ea-7e97a81e1118.png)

122. Click **Designer**

123. Click **More Action** Icon for **Account**

124. Click **Add Calculation**

![10-92](https://user-images.githubusercontent.com/92877810/141184259-6c50aea8-59d2-4e8d-b203-b379e11cb3e0.png)

125. Click **Date Difference**

![10-93](https://user-images.githubusercontent.com/92877810/141184261-e5ff9630-0efc-4639-be65-44305066cf75.png)

The time to deliver the orders is the difference between Receive Date and Order Date. 

126. Expand **Time (A)**

127. Click **Receive Date**

![10-94](https://user-images.githubusercontent.com/92877810/141184263-dc431ac6-af78-4ef1-afa7-ad3f2bd307d2.png)

🚩You must specify the context of the calculation. As the delivery time is based on orders you must use Order ID in the dimension context. Also, in case the chart or table does not include Order ID, then an additional average aggregation will be applied to the calculation.  

128. Expand **Dimension Context**

![10-95](https://user-images.githubusercontent.com/92877810/141184264-9fd19f71-1006-41d0-b64b-b2248ec77e9f.png)

129. Click **Order ID**

130. Click Outside the Dimension Context Drop Down Menu to Collapse

![10-96](https://user-images.githubusercontent.com/92877810/141184266-f4134e2a-b166-43ef-96a3-96dba5d28d88.png)

131. Rename Calculation to **Delivery Time**

132. Click **OK**

![10-97](https://user-images.githubusercontent.com/92877810/141184267-048c4d0d-2b30-4780-baf4-b8f707e804a3.png)

🚩You can see the delivery time has been added to the table.  
  
**Note:** You may need to scroll in the table to see the new calculation. 

![10-98](https://user-images.githubusercontent.com/92877810/141184268-8c1b9f9f-0a49-4348-89ef-1683ab453280.png)
  
Let's format the calculation. 

133. Click **1 Story Calculations**

134. Click **Edit Formatting**

![10-99](https://user-images.githubusercontent.com/92877810/141184269-dfec9bf3-534d-45ed-b945-20795ad2a8f9.png)

135. Deselect **Use Unit of Underlying Measure**

136. Set **Decimal Places** to **0**

137. Click **OK**

![10-100](https://user-images.githubusercontent.com/92877810/141184270-15b92fc8-eae2-4252-897b-03b84866052f.png)

🚩The calculation has been formatted. Let's order the measures in the table. 

![10-101](https://user-images.githubusercontent.com/92877810/141184272-8fe47644-d760-484c-b51b-e25261d0eb83.png)

138. Click **Designer** to collapse the **Designer Panel**

![10-102](https://user-images.githubusercontent.com/92877810/141184274-614deefe-1377-4a42-be47-18fdb3eaa4b8.png)

🚩We want to reorder the measure within our table. 

139. Right Click on **Account**  to Open the Context Menu

140. Click **Sort Options**

141. Click **Add Custom Order**

![10-103](https://user-images.githubusercontent.com/92877810/141184275-bb63c680-1269-46cd-9aaa-bd536fda883d.png)

🚩The desired order is: 
•	Delivery Time 
•	Sales Revenue 
•	Gross Margin 
•	Discount 

142. Click and Drag Delivery Time to the top

143. Click and drag Sales Renue Below Delivery Time

144. Click and Drag Gross Margin above Discount

![10-104](https://user-images.githubusercontent.com/92877810/141184278-bb131b96-2415-4be4-a829-d1262ef7b444.png)

⚠️Quality Check! Does your custom sort match the screenshot? 

145. Click **OK**

![10-105](https://user-images.githubusercontent.com/92877810/141184279-a7db2c5e-27a0-4e06-af94-8f36f68df776.png)

⚠️Quality Check! Does your table look like this?

![10-106](https://user-images.githubusercontent.com/92877810/141184280-5817c42f-bbb4-4ac6-a5be-958cd2a54488.png)

🚩Next you want to compare the financial performance for this year to the performance from last year during the same period. You will do the analysis on the Financial Performance table. Select the table and open the Builder panel.  

146. Scroll to the **Bottom** of the Dashboard

147. Click the **Financial Performance** Table

![10-107](https://user-images.githubusercontent.com/92877810/141184281-33f37b68-2a27-432e-959e-678ce907443f.png)

148. Click **Designer** to Open the Builder Panel

🚩The table uses a measure input control. You want to have the time calculations apply automatically to any measures in the table, this can be done using Cross Calculations. Add the Cross Calculation dimension to the table

149. Click **+ Add Measures/Dimensions**

![10-108](https://user-images.githubusercontent.com/92877810/141184282-6f228ea2-a01f-45d2-aa0a-fd44127d2c88.png)

150. Click **Cross Calculations**

151. Click **Outside** the **Measures/Dimensions** Drop Down Menu to Collapse

![10-109](https://user-images.githubusercontent.com/92877810/141184283-2b1bf5dc-0f4a-4af2-a115-34195d47fd5a.png)

🚩Let's add the first cross calculation as a restricted measure for the year to date time range using order date dimension 

152. Click the **More Actions** Icon for **Cross Calculations**

153. Click **Add Calculations**

![10-110](https://user-images.githubusercontent.com/92877810/141184284-7a3b1678-a191-4a90-abb7-028470f4102c.png)

154. Click **Restricted Measure**

![10-111](https://user-images.githubusercontent.com/92877810/141184285-d71a799e-fafe-403d-b690-8d5d2920309f.png)

155. Expand **Dimensions**

156. Click **Order Date**

![10-112](https://user-images.githubusercontent.com/92877810/141184286-0bd90e5a-5c52-479f-ac34-aebcbef4789c.png)

157. Expand **Values** or **Input Controls**

158. Expand **To Date** Under **Current Period**

![10-113](https://user-images.githubusercontent.com/92877810/141184287-76b55e49-17ae-4e86-8ced-dcbb7bc96490.png)

159. Click **Year**

![10-114](https://user-images.githubusercontent.com/92877810/141184288-071b9252-577b-4b53-aab2-9489a1bdcaea.png)

160. Rename the Calculation to **YTD**

161. Click **OK**

![10-115](https://user-images.githubusercontent.com/92877810/141184289-3eec058a-c9a3-480d-b973-721169b300f2.png)

🚩You can see the calculation was added to the table. Let's create an equivalent calculation for the previous year's value. 

![10-116](https://user-images.githubusercontent.com/92877810/141184291-9e79cb1c-0ec2-4d96-a0d7-90bbbfe6395b.png)

162. Click **Add Calculations**

163. Click the **More Action** Icon for **Cross Calculations**

![10-117](https://user-images.githubusercontent.com/92877810/141184294-34234e18-972f-4eac-8f24-0bd33bcf921c.png)

164. Click **Restricted Measure**

![10-118](https://user-images.githubusercontent.com/92877810/141184296-2b7912a9-9ef5-47c4-97f8-3a336fa72324.png)

165. Expand **Measures**

166. Click **Account Values**

![10-119](https://user-images.githubusercontent.com/92877810/141184297-b1732ab8-ccac-4df3-98ea-17a1d0e734c1.png)

167. Expand **Dimensions**

168. Click **Order Date**

![10-120](https://user-images.githubusercontent.com/92877810/141184299-3194d565-92ad-4e83-960e-e19dd54ddd8f.png)

169. Expand **Values** or **Input Controls**

170. Expand **To Date** Under **Previous Period**

171. Click **Year**

![10-121](https://user-images.githubusercontent.com/92877810/141184300-5299d513-4dc9-438f-8e9d-1b6a3a2e21b9.png)

172. Rename the Calculation to **PYTD**

173. Click **OK**

![10-122](https://user-images.githubusercontent.com/92877810/141184302-9134fd87-2183-4cc1-888e-2503c15331c0.png)

🚩Next you want to calculate the variance between last years data and this year’s data. 

174. Click the **More Actions** Icon for **Cross Calculations**

175. Click **Add Calculation**

![10-123](https://user-images.githubusercontent.com/92877810/141184303-6bf10815-a8f7-4fa1-948b-1bce81b45790.png)

176. Click **Calculated Measure**

![10-124](https://user-images.githubusercontent.com/92877810/141184306-536b840c-d466-4690-a843-a0f418997ef2.png)

177. Type **P**

178. Click **PYTD**

![10-125](https://user-images.githubusercontent.com/92877810/141184308-cf38271e-d029-40c0-a371-146e1f5a6e91.png)

179. Type **Y**

180. Click **- YTD** 

![10-126](https://user-images.githubusercontent.com/92877810/141184309-f6be7cad-a777-4568-8005-457e1c60d44b.png)

181. Rename Calculation to **Variance**

182. Click **OK**

![10-127](https://user-images.githubusercontent.com/92877810/141184310-13239b30-fafa-487c-a340-654c7c9ca077.png)

🚩Before reviewing the table. Let's make sure we have only the desired calculations selected. 

183. Click **Filter** for **Cross Calculations**

![10-128](https://user-images.githubusercontent.com/92877810/141184311-15e4e02c-854e-47cc-beed-9fdb36997051.png)

184. Click **PYTD**

185. Click **OK**

![10-129](https://user-images.githubusercontent.com/92877810/141184312-4c6e3b60-9055-4db0-a832-518ea2ed9f94.png)

⚠️Quality Check! Does your table look like this? 
  
Note: Due to the dynamic time filter the data may vary. 

![10-130](https://user-images.githubusercontent.com/92877810/141184315-0e91f804-f09e-4e57-835c-fd6e2e396422.png)

🚩Next, you would like to adjust the order of the columns in the table. 

186. Click the **More Actions** Icon for **Cross Calculations**

187. Click **Edit Member Order...**

![10-131](https://user-images.githubusercontent.com/92877810/141184316-920ef0e2-cf7e-4c3d-a170-3cc7b002c88e.png)

🚩The required member order is: 
 
YTD
PYTD
Variance
Account Values
Measure Selector

188. Click and drag **YTD** to top

189. Click and drag **PYTD** below YTD

190. Click and drag **Variance** below PYTD

![10-132](https://user-images.githubusercontent.com/92877810/141184317-d8a36b10-5f05-4873-b86d-33b2b536ae68.png)

⚠️Quality Check! Does your Edit Member Order match the screenshot? 

191. Click **Done**

![10-133](https://user-images.githubusercontent.com/92877810/141184319-b7576665-3720-48e4-a7a6-20c3749205e3.png)

⚠️Quality Check! Does your table look like this? 

![10-134](https://user-images.githubusercontent.com/92877810/141184320-bc39721c-63b9-4c13-841b-6c11fe3f4525.png)

🚩You want to make the variance stand out more easily indicating where there was an increase or decrease from last year. This can easily be done by turning it into a variance in-cell chart.  

192. Right Click Variance to Open the Context Menu

193. Click **In-Cell Chart**

![10-135](https://user-images.githubusercontent.com/92877810/141184322-150fefd7-66fe-49d6-8796-1e51f719d519.png)

194. Click the **In-Cell Chart**

195. Expand the **Comparison Tile**

196. Click **Variance Bar**

![10-137](https://user-images.githubusercontent.com/92877810/141184324-57f91e53-435a-4229-b3a0-220fbac8c63e.png)

⚠️Quality Check! Does your table look like this? 

![10-138](https://user-images.githubusercontent.com/92877810/141184325-1e1b1b8b-a078-46c9-ae97-d6acb7e05f6e.png)

🚩Next let's look at some time navigation inside a chart. The chart shows the Sales Revenue over time. Let's drill a level down to understand how 2021 is performing. 

197. Drag the **Horizontal Scroll Bar** to the **Right**

198. Left Click the **2021** Bar

199. Click the **Drill Down** Icon

![10-139](https://user-images.githubusercontent.com/92877810/141184327-c87b56e8-9acf-4418-bf3f-65fdc23eabd8.png)

🚩You can see the chart now show the Sales Revenue by quarter. However, you're more interested in it for the half year. Let's change the hierarchy via the builder panel. 

![10-140](https://user-images.githubusercontent.com/92877810/141184328-9e0afe56-c63d-4e2b-9d18-7714fd86172b.png)

200. Click the **Drill** Icon for **Order Date**

201. Click **Set Hierarchy**

![10-141](https://user-images.githubusercontent.com/92877810/141184331-2529667e-a6ab-4448-9f6a-3aefa8495b21.png)

202. Expand **Hierarchy**

203. Click **Year, Half-Year, Quarter, Month, Day**

![10-142](https://user-images.githubusercontent.com/92877810/141184334-c1392574-175e-48cf-bfb7-291623bb3b88.png)

204. Click **Set**

![10-143](https://user-images.githubusercontent.com/92877810/141184337-327a5e6c-a9db-4c1d-9337-760f21a8dbe5.png)

🚩The chart has been reset to the new hierarchy. Let's change the level via the builder panel. 

![10-144](https://user-images.githubusercontent.com/92877810/141184338-264f53a6-fe9c-4b68-badb-4fb9cdf3a5e1.png)

205. Click the **Drill Icon** for **Order Date**

206. Click **Level 3**

![10-145](https://user-images.githubusercontent.com/92877810/141184339-0983234e-fa37-4a19-8c7a-5dfc594bf5d4.png)

⚠️Quality Check! Does your chart look like this? 

![10-146](https://user-images.githubusercontent.com/92877810/141184341-abdac089-4a9b-41e2-a084-2a67e3b022db.png)

🚩Now let's look at quickly showing the year over year changes if the Sales Revenue. This can be done via time calculation quick options if time if in the chart

207. Click the **More Action Icon** for **Sales Revenue** under Measures

![10-147](https://user-images.githubusercontent.com/92877810/141184342-b5402795-6802-48a2-9d11-f7541f4b9629.png)

208. Click **Add Time Calculation**

209. Click **Year Over Year**

![10-148](https://user-images.githubusercontent.com/92877810/141184343-83d75052-8c2a-4697-add5-17e5d76bfa92.png)

210. Remove **Sales Revenue**

![10-149](https://user-images.githubusercontent.com/92877810/141184344-5f6466df-2c07-4a50-8f12-c511b95f2a1c.png)

⚠️Quality Check! Does your chart look like this? 

![10-150](https://user-images.githubusercontent.com/92877810/141184345-5858f7d9-0e56-4305-a241-30a59f527c32.png)

🚩You can see that H1 2021 is significantly lower than H1 2020. Let's drill into this more. 

211. Click the **H1 2021** Bar

212. Click **Drill Down**

![10-151](https://user-images.githubusercontent.com/92877810/141184346-8e371521-c693-4f3a-bad1-fe500e72c068.png)

🚩The major deviation was in Q1 of 2021. 

![10-152](https://user-images.githubusercontent.com/92877810/141184348-4f95f491-f7a1-4ce2-a007-5c075bbd53a1.png)
  
ℹ️You have concluded the **Time Analysis Section!** Save your document.

🚩Press **Ctrl + S** to save your story

![10-f](https://user-images.githubusercontent.com/92877810/141187198-b36b5cd0-8bbd-4111-a386-16cea2ca8b4f.png)

<br><br>

## Summary

**You have completed the entire Time Analysis section!**

**You are now able to:**
- Create dynamic and fixed date-based story and page filters with multiple ranges
- Customise “current date” for greater flexibility when analysing time-based data
- Create dynamic calculations such as Year-to-Date (YTD), Previous Year-to-Date (PYTD) and others
- Define date-based hierarchies in SAC that best suit your needs

