⚠️Quality Check! Does your screen look like this screenshot?

![10-1](https://user-images.githubusercontent.com/92877810/140169050-9da1077e-80d2-4de4-a035-b10a445bca10.png)

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

🚩You can see the Date Selector input control was added to the story filter bar. In the time series chart, you can see that the data now show November data until November 30th

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
