# Section 10 - Time Analysis

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

![10-30](https://user-images.githubusercontent.com/92877810/140178417-c7566064-7259-4ad5-b9ac-2bbc7b298b7c.png)

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

![10-35](https://user-images.githubusercontent.com/92877810/140178425-5a8089ae-8aab-460b-8777-38380541b6b7.png)

🚩You can see on the time series chart that the filter has been applied. Let's extend to view the last 2 years as well as the current year. 

![10-36](https://user-images.githubusercontent.com/92877810/140178427-3abdf64d-17f0-44eb-969e-0c8cff1fca4d.png)

51. Click **Current Month**

52. Click the **Last Member**

53. Click  outside to collapse the story filter

![10-37](https://user-images.githubusercontent.com/92877810/140178429-9a41f6f6-996a-43c6-ab55-0b79d807b7c7.png)

🚩Again, you can see on the time series chart that the filter has been applied.  

![10-38](https://user-images.githubusercontent.com/92877810/140178431-5350fbe1-7f30-4d37-83d2-97e1a6fcc0f0.png)

🚩Right now, the story filter has still a lot of options such as configuring the time periods to go back to. You can hide this complexity from the story viewer. Let's do that and only expose the effected time range to the story viewers. 

54. Click **Current Month**

55. Click **Settings**

56. Click **Show/Hide**

![10-39](https://user-images.githubusercontent.com/92877810/140178433-75828487-bca8-48f4-b89a-48203e0e623c.png)

57. Deselect **Look Back**

58. Deselect **Current Period**

59. Deselect **Look Ahead**

60. Deselect **Range Info Icons**

![10-40](https://user-images.githubusercontent.com/92877810/140178440-9bee5706-6d6e-4e64-b69f-3fbf24ac70e6.png)

🚩You can see that this looks much cleaner. 

![10-41](https://user-images.githubusercontent.com/92877810/140178442-81320b5e-7c34-4b03-8118-c6eb410efbdb.png)

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

105. Drag.

106. Drop on .

![10-79](https://user-images.githubusercontent.com/92877810/140186495-df666425-8c9b-46de-baee-946d40fe5d16.png)

🚩You may have noticed that the entire dashboard is filtered on the Order and Receive date input controls that you just added. You only want to apply these to the Order Delivery Analysis table. You can use Linked Analysis to set the scope of the page input controls

107. Click the **Order Date Range Filter**

108. Click the **More Action**

109. Click **Linked Analysis**

![10-80](https://user-images.githubusercontent.com/92877810/140186496-6ae5f811-92d1-429c-aa2c-7512086976a2.png)

110. Click **Only Selected Widgets**

![10-81](https://user-images.githubusercontent.com/92877810/140186497-bc428b4a-08ec-4967-b407-95b70f040a89.png)

111. Scroll and Click **Order Delivery Analysis**

112. Click **Apply**

![10-82](https://user-images.githubusercontent.com/92877810/140186499-1133a61e-128c-4c29-a45e-ea12dee51c60.png)

🚩We want to repeat the steps for the 
Receive Date Range Filter Input Control. 

113. Click **Receive Date Range Filter**

114. Click **More Action** icon

115. Click **Linked Analysis**

![10-83](https://user-images.githubusercontent.com/92877810/140186502-56325139-6b98-4598-b773-50cb9156239a.png)

116. Click **Only Selected Widgets**

![10-84](https://user-images.githubusercontent.com/92877810/140186505-b049e077-4c88-451d-a02c-7f8845672c1f.png)

117. Scroll and Click **Order Delivery Analysis**

118. Click **Apply**

![10-85](https://user-images.githubusercontent.com/92877810/140186506-6bdc613a-d4c1-441b-8fa4-26c45bc90d11.png)

⚠️Quality Check! Your page input controls should only drive the Order Delivery Analysis table

![10-86](https://user-images.githubusercontent.com/92877810/140186509-4a1a1cf7-3315-44e7-9275-15a046d644d1.png)

🚩Let's find out which orders that were shipped after Oct 1st, 2021 have been received by October 8th, 2021. 

119. Click the **End Date Picker**

![10-87](https://user-images.githubusercontent.com/92877810/140186512-413438e7-b011-4fc5-b628-15776b63e818.png)

120. Click **November**

![10-88](https://user-images.githubusercontent.com/92877810/140186513-3c465b16-965c-461a-9eb2-26874113e9fe.png)

121. Click **Oct**

![10-89](https://user-images.githubusercontent.com/92877810/140186514-fc5e9d28-a1aa-4c8f-b308-9ceab2ac1f01.png)

122. Click **8**

![10-90](https://user-images.githubusercontent.com/92877810/140186516-b102e2c1-4cac-49c3-bc40-18bb289abce6.png)
  
🚩Next you want to calculate the time it takes to deliver your orders. This can easily be done via calculations. 

123. Click the **Order Delivery Analysis Table**

![10-91](https://user-images.githubusercontent.com/92877810/140186519-db3becca-215f-4e71-aa49-2f30a4ad8222.png)

124. Click **Designer**

125. Click **More Action** Icon for **Account**

126. Click **Add Calculation**

![10-92](https://user-images.githubusercontent.com/92877810/140186521-6a21f910-e8ab-43a2-b8bf-0a5289473498.png)

127. Click **Date Difference**

![10-93](https://user-images.githubusercontent.com/92877810/140186522-6b19ff77-090d-4095-9052-b5074fdea4e2.png)

The time to deliver the orders is the difference between Receive Date and Order Date. 

128. Expand **Time (A)**

129. Click **Receive Date**

![10-94](https://user-images.githubusercontent.com/92877810/140186524-d499a9d0-c42b-49fa-81ed-4ca4875c0614.png)

🚩You must specify the context of the calculation. As the delivery time is based on orders you must use Order ID in the dimension context. Also, in case the chart or table does not include Order ID, then an additional average aggregation will be applied to the calculation.  

130. Expand **Dimension Context**

![10-95](https://user-images.githubusercontent.com/92877810/140186525-f3c28564-d364-48de-ac19-5c2ea740c655.png)

131. Click **Order ID**

132. Click Outside the Dimension Context Drop Down Menu to Collapse

![10-96](https://user-images.githubusercontent.com/92877810/140186527-ce60798c-380d-4fd7-82ae-5e4d74aa9a52.png)

133. Rename Calculation to **Delivery Time**

134. Click **OK**

![10-97](https://user-images.githubusercontent.com/92877810/140186528-fc880f7e-7fa9-48d8-afe1-b8ca316fd413.png)

🚩You can see the delivery time has been added to the table.  
  
**Note:** You may need to scroll in the table to see the new calculation. 

![10-98](https://user-images.githubusercontent.com/92877810/140186530-2f9ea854-9ce7-4bfa-b63c-1874b981f206.png)
  
Let's format the calculation. 

135. Click **1 Story Calculations**

136. Click **Edit Formatting**

![10-99](https://user-images.githubusercontent.com/92877810/140186533-5ed7d0e2-7907-4d2f-ade6-0a020f0a0980.png)

137. Deselect **Use Unit of Underlying Measure**

138. Set **Decimal Places** to **0**

139. Click **OK**

![10-100](https://user-images.githubusercontent.com/92877810/140186534-4efe053f-b133-4ac8-8219-b129a6b03561.png)

🚩The calculation has been formatted. Let's order the measures in the table. 

![10-101](https://user-images.githubusercontent.com/92877810/140192554-52e3153d-fcc2-45c4-a3d9-76c0a3809f28.png)

140. Click **Designer** to collapse the **Designer Panel**

![10-102](https://user-images.githubusercontent.com/92877810/140192558-60a7965c-13a9-4045-bb89-78dc0c4e3b51.png)

🚩We want to reorder the measure within our table. 

141. Right Click on **Account**  to Open the Context Menu

142. Click **Sort Options**

143. Click **Add Custom Order**

![10-103](https://user-images.githubusercontent.com/92877810/140192559-a781153e-976c-49f3-a326-ee2ec079abf7.png)

🚩The desired order is: 
•	Delivery Time 
•	Sales Revenue 
•	Gross Margin 
•	Discount 

144. Click and Drag Delivery Time to the top

145. Click and drag Sales Renue Below Delivery Time

146. Click and Drag Gross Margin above Discount


![10-104](https://user-images.githubusercontent.com/92877810/140192561-efc8a051-1b8b-4120-8b64-008281c08396.png)

⚠️Quality Check! Does your custom sort match the screenshot? 

147. Click **OK**

![10-105](https://user-images.githubusercontent.com/92877810/140192562-b3658ddd-593f-46c0-b408-caff6446e3b2.png)

⚠️Quality Check! Does your table look like this? 

![10-106](https://user-images.githubusercontent.com/92877810/140192564-6787222a-eb94-41f2-8cf8-801fb60c3ed7.png)

🚩Next you want to compare the financial performance for this year to the performance from last year during the same period. You will do the analysis on the Financial Performance table. Select the table and open the Builder panel.  

148. Scroll to the **Bottom** of the Dashboard

149. Click the **Financial Performance** Table

![10-107](https://user-images.githubusercontent.com/92877810/140192565-ed098374-0244-4848-bc0f-4f6f30c0a3e5.png)

150. Click **Designer** to Open the Builder Panel

🚩The table uses a measure input control. You want to have the time calculations apply automatically to any measures in the table, this can be done using Cross Calculations. Add the Cross Calculation dimension to the table

151. Click **+ Add Measures/Dimensions**

![10-108](https://user-images.githubusercontent.com/92877810/140192566-b5a7f715-50e5-4f6b-b47b-b212b9046f44.png)

152. Click **Cross Calculations**

153. Click **Outside** the **Measures/Dimensions** Drop Down Menu to Collapse

![10-109](https://user-images.githubusercontent.com/92877810/140192567-969736ce-018a-4609-b7ad-c0e3c57be954.png)

🚩Let's add the first cross calculation as a restricted measure for the year to date time range using order date dimension 

154. Click the **More Actions** Icon for **Cross Calculations**

155. Click **Add Calculations**

![10-110](https://user-images.githubusercontent.com/92877810/140192569-7cb06df7-d840-4f8c-bb9b-b85ffcfbf01f.png)

156. Click **Restricted Measure**

![10-111](https://user-images.githubusercontent.com/92877810/140192570-2c242cbe-166d-42e1-974d-ca2b060cf4be.png)

157. Expand **Dimensions**

158. Click **Order Date**

![10-112](https://user-images.githubusercontent.com/92877810/140192572-038cff7b-7a9a-41a6-9347-6c1184af9098.png)

159. Expand **Values** or **Input Controls**

160. Expand **To Date** Under **Current Period**

![10-113](https://user-images.githubusercontent.com/92877810/140192574-d0633bf1-1ce7-420c-9be4-51be75267a7f.png)

161. Click **Year**

![10-114](https://user-images.githubusercontent.com/92877810/140192575-2bf06b8a-c437-487d-8c57-bb010c217fd5.png)

162. Rename the Calculation to **YTD**

163. Click **OK**

![10-115](https://user-images.githubusercontent.com/92877810/140192577-8bb7976b-f5d6-4437-bd00-45199200fccc.png)

🚩You can see the calculation was added to the table. Let's create an equivalent calculation for the previous year's value. 

![10-116](https://user-images.githubusercontent.com/92877810/140192579-4a5a9b6d-69fb-409b-ac40-6eca1eb26f0d.png)

164. Click **Add Calculations**

165. Click the **More Action** Icon for **Cross Calculations**

![10-117](https://user-images.githubusercontent.com/92877810/140192580-1a3af021-a454-44ce-8ab8-1c858d24458a.png)

166. Click **Restricted Measure**

![10-118](https://user-images.githubusercontent.com/92877810/140192582-103f71f8-2f78-4ed6-995a-0c5bbab1db9c.png)

167. Expand **Measures**

168. Click **Account Values**

![10-119](https://user-images.githubusercontent.com/92877810/140192584-d2bf122b-e877-4e9c-8d5c-611ed64c7fa9.png)

169. Expand **Dimensions**

170. Click **Order Date**

![10-120](https://user-images.githubusercontent.com/92877810/140192585-c3bfd93c-2db9-4682-aa36-71d60f3b5c36.png)

171. Expand **Values** or **Input Controls**

172. Expand **To Date** Under **Previous Period**

173. Click **Year**

![10-121](https://user-images.githubusercontent.com/92877810/140194901-16dd988d-2aa2-453d-a363-8e7e0609d3f5.png)

174. Rename the Calculation to **PYTD**

175. Click **OK**

![10-122](https://user-images.githubusercontent.com/92877810/140194904-f1fa64e4-cffe-4c9d-9877-70cf030cc428.png)

🚩Next you want to calculate the variance between last years data and this year’s data. 

176. Click the **More Actions** Icon for **Cross Calculations**

177. Click **Add Calculation**

![10-123](https://user-images.githubusercontent.com/92877810/140416150-41033377-251d-4973-88be-b0e5a24b1c64.png)

178. Click **Calculated Measure**

![10-124](https://user-images.githubusercontent.com/92877810/140416151-09429935-49d8-4c60-9655-8e83e7976ef8.png)

179. Type **P**

180. Click **PYTD**

![10-125](https://user-images.githubusercontent.com/92877810/140416153-846fedb2-0554-4521-bdbd-8a956afd2de6.png)

181. Type **Y**

182. Click **YTD** 

![10-126](https://user-images.githubusercontent.com/92877810/140416155-e4d922c4-1a30-43cd-829e-fcf8a261f88f.png)

183. Rename Calculation to **Variance**

184. Click **OK**

![10-127](https://user-images.githubusercontent.com/92877810/140416156-8846a57c-5104-40ec-b19d-9931310db939.png)

🚩Before reviewing the table. Let's make sure we have only the desired calculations selected. 

185. Click **Filter** for **Cross Calculations**

![10-128](https://user-images.githubusercontent.com/92877810/140416158-559e4385-de9b-4070-be7b-2c3f6b8b73da.png)

186. Click **PYTD**

187. Click **OK**

![10-129](https://user-images.githubusercontent.com/92877810/140416160-73313292-70eb-4644-899f-39044fe52708.png)

⚠️Quality Check! Does your table look like this? 
  
Note: Due to the dynamic time filter the data may vary. 

![10-130](https://user-images.githubusercontent.com/92877810/140416162-7629fd39-d437-4c9d-8780-772c0f9df1df.png)

🚩Next, you would like to adjust the order of the columns in the table. 

188. Click the **More Actions** Icon for **Cross Calculations**

189. Click **Edit Member Order...**

![10-131](https://user-images.githubusercontent.com/92877810/140416163-f8f3c2d3-03e7-4132-a3b0-6b3c1fb2a75f.png)

🚩The required member order is: 
 
YTD
PYTD
Variance
Account Values
Measure Selector

190. Click and drag **YTD** to top

191. Click and drag **PYTD** below YTD

192. Click and drag **Variance** below PYTD

![10-132](https://user-images.githubusercontent.com/92877810/140416164-e41aecd9-f4e5-490c-92c7-2bcf8f57d885.png)

⚠️Quality Check! Does your Edit Member Order match the screenshot? 

193. Click **Done**

![10-133](https://user-images.githubusercontent.com/92877810/140416166-20d56089-9df8-4757-ba13-3cebc3e046e8.png)

⚠️Quality Check! Does your table look like this? 

![10-134](https://user-images.githubusercontent.com/92877810/140416167-ff83c058-1b55-4cde-85a6-9c8a00be3419.png)

🚩You want to make the variance stand out more easily indicating where there was an increase or decrease from last year. This can easily be done by turning it into a variance in-cell chart.  

194. Right Click Variance to Open the Context Menu

195. Click **In-Cell Chart**

![10-135](https://user-images.githubusercontent.com/92877810/140416170-c0f79d3a-335d-4606-af6b-90e489445331.png)

196. Click the **In-Cell Chart**

197. Expand the **Comparison Tile**

198. Click **Variance Bar**

![10-137](https://user-images.githubusercontent.com/92877810/140416173-43fbea61-d361-43e3-820f-02393749ab99.png)

⚠️Quality Check! Does your table look like this? 

![10-138](https://user-images.githubusercontent.com/92877810/140416176-89626d1d-121a-4cf6-b421-277a580bd682.png)

🚩Next let's look at some time navigation inside a chart. The chart shows the Sales Revenue over time. Let's drill a level down to understand how 2021 is performing. 

199. Drag the **Horizontal Scroll Bar** to the **Right**

200. Left Click the **2021** Bar

201. Click the **Drill Down** Icon

![10-139](https://user-images.githubusercontent.com/92877810/140416177-73f0524d-dc6b-4f03-b4a3-e9c59ef80d3d.png)

🚩You can see the chart now show the Sales Revenue by quarter. However, you're more interested in it for the half year. Let's change the hierarchy via the builder panel. 

![10-140](https://user-images.githubusercontent.com/92877810/140416178-718fb807-8904-4739-a533-069d6b6a29ae.png)

202. Click the **Drill** Icon for **Order Date**

203. Click **Set Hierarchy**

![10-141](https://user-images.githubusercontent.com/92877810/140416179-ce6c7d10-0ad1-4402-9284-8ad2a3e86aee.png)

204. Expand **Hierarchy**

205. Click **Year, Half-Year, Quarter, Month, Day**

![10-142](https://user-images.githubusercontent.com/92877810/140416180-6997eec4-4e42-4aa4-add8-cf08b18c2765.png)

206. Click **Set**

![10-143](https://user-images.githubusercontent.com/92877810/140416182-ea251592-5015-414a-b23b-be56f4ad2444.png)

🚩The chart has been reset to the new hierarchy. Let's change the level via the builder panel. 

![10-144](https://user-images.githubusercontent.com/92877810/140416184-a9ba3c1a-fb15-4d23-a63c-9f9e703b811a.png)

207. Click the **Drill Icon** for **Order Date**

208. Click **Level 3**

![10-145](https://user-images.githubusercontent.com/92877810/140416186-68e5abb9-113e-43a0-89b8-ac0ba8acec11.png)

⚠️Quality Check! Does your chart look like this? 

![10-146](https://user-images.githubusercontent.com/92877810/140416190-11f22b89-2fde-4bf0-9082-a6a1e3ef2e2e.png)

🚩Now let's look at quickly showing the year over year changes if the Sales Revenue. This can be done via time calculation quick options if time if in the chart

209. Click the **More Action Icon** for **Sales Revenue** under Measures

210. Click **Add Time Calculation**

211. Click **Year Over Year**

![10-147](https://user-images.githubusercontent.com/92877810/140416191-3900cf0e-b912-4431-a5a8-23368a9e981a.png)

212. Remove **Sales Revenue**

![10-148](https://user-images.githubusercontent.com/92877810/140416193-480abdcc-9038-41c2-9c0f-86f7b6928272.png)

⚠️Quality Check! Does your chart look like this? 

![10-149](https://user-images.githubusercontent.com/92877810/140416194-6f6cdf60-7e4a-4a2a-aab7-7b13017ab304.png)

🚩You can see that H1 2021 is significantly lower than H1 2020. Let's drill into this more. 

213. Click the **H1 2021** Bar

214. Click **Drill Down**

![10-150](https://user-images.githubusercontent.com/92877810/140416197-cc7fce00-97b6-46b4-b384-e0163c0c0d1a.png)

🚩The major deviation was in Q1 of 2021. 

![10-151](https://user-images.githubusercontent.com/92877810/140416198-30c6cd7a-266b-4cbb-819a-d348a8073529.png)
  
ℹ️You have concluded the **Time Analysis Section!** Save your document.

🚩Press **Ctrl + S** to save your story

![10-152](https://user-images.githubusercontent.com/92877810/140416199-770e7da5-4f92-4a6d-b574-e7de1ba43228.png)

<br><br>

## Summary

**You have completed the entire Time Analysis section!**

**You are now able to:**
- Create dynamic and fixed date-based story and page filters with multiple ranges
- Customise “current date” for greater flexibility when analysing time-based data
- Create dynamic calculations such as Year-to-Date (YTD), Previous Year-to-Date (PYTD) and others
- Define date-based hierarchies in SAC that best suit your needs

