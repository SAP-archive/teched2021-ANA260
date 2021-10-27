# Section 7 - Performance Optimization

ℹ️**Objective:** Use Natural Language Search (Search to Insight) to translate your questions into visualizations 
and understand how to run a Smart Discovery within SAP Analytics Cloud. Develop an understanding and 
purpose of the various pages that are created by Smart Discovery.

**Estimated Time:** 15 mins

**Exercise Description:** After hearing back from your colleagues about the dashboard you shared, you have 
a few quick questions regarding the company’s financial. You can quickly find answers for your questions via 
Search to Insight, leveraging SAC’s natural language processing capabilities. Once you try Search to Insight 
for yourself, you can tell your colleagues all about it and they will no longer need to come to you with their 
questions about data. 

Once SAP Analytics Cloud found the answer to your questions you want to use other smart features such 
smart insight and time series forecast to enhance the result. Finally, you want to use Smart Discovery to 
have SAP Analytics Cloud investigate Gross Margin at BestRun and automatically built a story for you.

**Key Features:**
- Use Search to Insight to find answers for your questions with natural language
- Have SAP Analytics Cloud investigate one of the measures and build a dashboard for you with Smart Discovery
- Understand how Smart Insights can help you explain more of your data

⚠️**Disclaimer**
When completing exercises, some data values in the screenshots may not match what you see on your 
screen. This is because the dynamic time filters that were applied at the time the screenshots were taken is 
different from the current system date.

----------------------------------------------------------------------------------------------------------------------------------------

ℹ️**Quality Check!** Does your story look like this? 

![7-1](https://user-images.githubusercontent.com/92877810/139118586-5aa52e23-65d2-4ac7-bbeb-07b277dd9354.png)

🚩To make it easier, we have created a story for Performance Optimization for you to work on. 
 
Let's open the required story

1. Click **Files**

![7-2](https://user-images.githubusercontent.com/92877810/139118587-ff0f39d3-ab77-4035-923e-f12122ab6431.png)

2. Click **Public**

![7-3](https://user-images.githubusercontent.com/92877810/139118588-819a8cd2-570d-43dd-b715-0bd5570b2090.png)

3. Click **TechEd 2021**

![7-4](https://user-images.githubusercontent.com/92877810/139118589-a7b026a2-21f2-42c5-86cb-3418c3da537a.png)

4. Open **Section 7 - Perfromance Optimisation START**

![7-5](https://user-images.githubusercontent.com/92877810/139118590-4f673288-916c-4781-b4fc-74d005b958fd.png)

ℹ️**Quality Check!** Does your story look like this?

![7-6](https://user-images.githubusercontent.com/92877810/139118592-3cf13c8f-28d0-43aa-a3f9-c7b75e60a421.png)

🚩To make the file easy to access, first save the story in MyFiles using your Initials.

5. Click **File**

6. Click **Save**

7. Click **Save As...**

![7-7](https://user-images.githubusercontent.com/92877810/139118594-89430be8-b4a8-4d58-b110-d2b9d2ea2c1f.png)

8. Go to **MyFiles**

![7-8](https://user-images.githubusercontent.com/92877810/139118595-0086f14c-55b7-4104-91c4-b44093d6afe9.png)

9. Rename the File as **Section 7 - Performance Optimisation Your Initials**

![7-9](https://user-images.githubusercontent.com/92877810/139118596-bc5e3cb7-80db-4bf1-8d69-23f380a71ee3.png)

10. Click **Edit** to go into Edit mode

![7-10](https://user-images.githubusercontent.com/92877810/139118598-62f73223-4f25-4120-ad2b-fe3e85fefeeb.png)

🚩If you scroll down you see that you already have a lot of widgets present in this story.
 
Let's add another chart to this page.

![7-11](https://user-images.githubusercontent.com/92877810/139118599-7f7f0bc8-d7cd-47e9-96a9-79938c69d4a2.png)

11. Select the **Bottom Lane**

12. Click **Insert**

13. Click **Chart**

![7-12](https://user-images.githubusercontent.com/92877810/139118600-01d69e8d-44f3-4916-9d08-6b71bfe3fc07.png)

💡As you add a new chart, a new desginer only performance optimization tip appears.
 
This tip warns you that you already have a large number of widgets or the widget your story contains are complex and process-heavy. It suggests you to change the design of your page either by removing some widgets or changing their type. 
 
To make the performance better, remove some widgets from your story.
 
You can click on learn more to know more about this Performance Tip

![7-13](https://user-images.githubusercontent.com/92877810/139118601-e56064de-281f-4742-aaba-20aa455d992c.png)

14. Select the table 

15. Click **More** icon

16. Click **Remove**

![7-14](https://user-images.githubusercontent.com/92877810/139118602-310dd439-63e4-44b8-9dd8-a92550229ebe.png)

ℹ️**Notice!** The Performance Tip is no longer there once we remove the table.

![7-15](https://user-images.githubusercontent.com/92877810/139118603-285711db-c925-4881-b80c-edf493323680.png)

17. Select the chart

18. Move the chart here

![7-16](https://user-images.githubusercontent.com/92877810/139118604-a5d478a4-164e-4eff-8a2c-cab8a338f1b1.png)

19. Click **Designer** (if Builder Panel not already open)

20. Click **Add Measure**

![7-17](https://user-images.githubusercontent.com/92877810/139118606-829543d2-01f3-4648-b58c-3b472bb4bf05.png)

21. Scroll until you find Gross Margin

22. Select **Gross Margin**

23. Click outside the Builder Panel to collapse the Measure drop down menu

![7-18](https://user-images.githubusercontent.com/92877810/139121953-67e635a0-0c18-4ecb-920e-a3fd58946f3e.png)

24. Click **Add Dimension**

![7-19](https://user-images.githubusercontent.com/92877810/139121956-85b19dad-02f6-4ee5-ad77-2cc0de65eb97.png)

25. Scroll until you find Region

26. Click **Region**

27. Click outside the Builder Panel to collapse the Dimension drop down menu

![7-20](https://user-images.githubusercontent.com/92877810/139121958-a1417607-f1c6-421f-98e5-e3a5c4430cee.png)

28. Click **More** icon

29. Click **Rank**

30. Click **Region**

31. Click **Top 5**

![7-21](https://user-images.githubusercontent.com/92877810/139121962-716928e6-b5f6-4ad6-b2c2-a8d9803f5a46.png)

⚠️**Quality Check!** Does your chart look like this? 

![7-22](https://user-images.githubusercontent.com/92877810/139121963-157d6cfd-448b-41de-9178-64b86bc3ec20.png)

32. Click **More** icon

33. Click **Copy**

34. Click **Duplicate**

![7-23](https://user-images.githubusercontent.com/92877810/139121965-666c34fa-c016-4794-9c91-c29e61fb235c.png)

🚩**Notice!** You no longer have the optimization tip. Even though you added another chart and removed the table, you no longer have the performance tip. This is because the table was a heavier and more complex widget than a chart. Hence, it was impacting the performance of your story. 

![7-24](https://user-images.githubusercontent.com/92877810/139121966-6c5471c1-efb7-4536-9d89-d104f67b4df5.png)

35. Select the chart

36. Drag towards the right to make some room.

![7-25](https://user-images.githubusercontent.com/92877810/139121968-92a24f49-2e33-48f9-b630-8ff6d8c0d9ea.png)

37. Remove **Region**

![7-26](https://user-images.githubusercontent.com/92877810/139121969-0af603e1-8444-4baf-9a09-1a0ff4058fcf.png)

38. Click **Add Dimension**

![7-27](https://user-images.githubusercontent.com/92877810/139121971-773c0187-895f-47d5-80dd-bf072b682a96.png)

39. Scroll until you find Sales Manager

40. Select **Sales Manager**

41. Click outside the builder panel to collapse the Dimension drop down menu.

![7-28](https://user-images.githubusercontent.com/92877810/139121972-ad3ce7ce-8193-4e36-b6ea-ceec220fa3bf.png)

42. Click **More** icon

43. Click **Rank**

44. Click **Sales Manager**

45. Click **Top 5**

![7-29](https://user-images.githubusercontent.com/92877810/139121974-b93d7fe9-4288-4769-8886-5a8f5f54655f.png)

⚠️**Quality Check!** Does your story look like this?

![7-30](https://user-images.githubusercontent.com/92877810/139121975-68f98318-a6bb-47d0-a211-bd8325815845.png)

🚩Let's add a new Input Control to your story.

46. Scroll up to the **Second Lane** 

47. Select the **Second Left Lane**

![7-31](https://user-images.githubusercontent.com/92877810/139121977-9851d52f-bf23-4515-94ba-dcee9697f33e.png)

48. Click **Insert** 

49. Click **Input Control**

![7-32](https://user-images.githubusercontent.com/92877810/139121979-cc145f1f-b835-4d7b-973a-4cba4e2d35a4.png)

50. Click **Page Filter**

51. Click **Dimensions**

52. Select **Order Number**

![7-33](https://user-images.githubusercontent.com/92877810/139121981-9d7a5fb1-bae8-4f5b-98fd-ab7ccea0feef.png)

53. Click **All Members**

54. Click **OK**

![7-34](https://user-images.githubusercontent.com/92877810/139121982-7d797a3c-1743-42da-a0ac-462c4b47777a.png)

55. Expand the new Input Control

![7-35](https://user-images.githubusercontent.com/92877810/139121985-3828be45-fffb-4aee-a550-0ac72d26add9.png)

💡As you expand the new Input Control, you see there is a new Performance Tip. It is notifying you that because you created a dimension or page Input Control on a hierarchical dimension or a high cardinality dimension (a dimension that has a lot of dimension members), you are slowing down the performance of the story by expanding the Input Control.

![7-36](https://user-images.githubusercontent.com/92877810/139121987-edd5eaa3-686f-4141-9e3b-a6fade4b3cd9.png)

56. To improve the performance of your story, let's collapse the Input Control

ℹ️With the Input Control Collapsed, Dimension members will only be loaded on demand once a viewer selects input control.

![7-37](https://user-images.githubusercontent.com/92877810/139121989-96386c94-9bf7-4b0b-8e7c-488b87f5e613.png)

🚩Now if you notice, we have our Performance Optimization Tip on having too many widgets come back. 

![7-38](https://user-images.githubusercontent.com/92877810/139121990-ed50e6b1-d226-43ff-8305-3f4d3809c903.png)

57. Scroll to the bottom

58. Select the second chart we created

59. Click **More** icon

60. Click **Copy**

61. Click **Copy**

![7-39](https://user-images.githubusercontent.com/92877810/139121992-1349e6a9-1c0f-493f-bb55-d86180e9ac92.png)

62. Click **More** icon

63. Click **Remove**

![7-40](https://user-images.githubusercontent.com/92877810/139121993-9ead62d6-552e-4ca0-9c4a-582fc930a81a.png)

64. Click **Add New Page**

65. Click **Responsive**

![7-41](https://user-images.githubusercontent.com/92877810/139121994-e896a008-ad15-4268-8652-3e1b550b416c.png)

66. Click **File**

67. Click **Copy and Paste**

68. Click **Paste**

![7-42](https://user-images.githubusercontent.com/92877810/139121995-f5a0b426-eacd-46d3-a408-f86c7bd913e5.png)

🚩By copying the widget to a different page, you are not impacting the performance of the first page and still able to convey the information you want to. 

![7-43](https://user-images.githubusercontent.com/92877810/139121996-27a32a94-ddc9-4796-8bd3-e7ca50d2ac8f.png)

69. Hover over on the **Add New page** button
  
💡Now if you try add another page to the story, you will see a new Optimization Tip. It is letting you know that you now already have a lot of pages in the story and it may impact the story's performance if you add an additional page. 
 
In this case the story designer will always see the Perfromance Optimization Tip pop-up whenever there is more than 10 pages in a story.
 
We recommend not going against the performance tips for the best performance of your story.  

![7-44](https://user-images.githubusercontent.com/92877810/139121997-5278691d-fc9f-4fee-87a3-6891dc9bf43e.png)

🚩Now let's save your story

70. Click **File** 

71. Click **Save**
  
🚩**Notice!** As you go into Save Menu, you now see a new Optimization View Mode Enablement feature

![7-45](https://user-images.githubusercontent.com/92877810/139121999-9883b4ad-9cfc-4877-8aec-631daca7ddc9.png)

72. As you hover over the information icon, it is letting you know that you now have a new Optimized View Mode available that includes performance and usability improvements for your viewers.

![7-46](https://user-images.githubusercontent.com/92877810/139122001-199641cc-bfd8-4e59-9678-8a12a08fe375.png)

73. Let's enable the Optimized View Mode by clicking on it.   

![7-47](https://user-images.githubusercontent.com/92877810/139122003-e9bd3557-db6f-40c6-a211-28f2aede6c0b.png)

74. Click **File**

75. Click **Save**

76. Click **Save**

![7-48](https://user-images.githubusercontent.com/92877810/139122005-61ceaa65-870a-4602-b51b-88dc222a4a5e.png)

77. Click **Overview**

![7-49](https://user-images.githubusercontent.com/92877810/139122006-5eefe953-e0c3-4a5f-8b05-94ac4f9a36ca.png)

78. Click **View** to go into View Mode

![7-50](https://user-images.githubusercontent.com/92877810/139122012-f73e9900-bd0c-4784-b599-6643a4de064f.png)

ℹ️In Optimized View Mode, a new feature "Ghost Loading Indicator" is added. 
 
Dashboards now display an animated ghost widget, while data from the server is retrieved. It provides the story viewer an early insight to the type of visualization that is rendering and makes it easier to tell which objects are loading especially when they are small.

![7-51](https://user-images.githubusercontent.com/92877810/139122013-0fbc4b14-d9ae-41fc-9d53-d75ea56a027a.png)

ℹ️**Welcome to Optimized View Mode!**
 
With the latest release of SAP Analytics Cloud (2021.14 – Q3 QRC), we are introducing Optimized View Mode. It can be enabled on a per dashboard basis providing several usability improvements and a more performant dashboard (in certain scenarios).
 
We are constantly striving to provide a better experience to the viewer. Hence, Optimized View Mode addresses several usability challenges that have been raised by customers

![7-52](https://user-images.githubusercontent.com/92877810/139122015-280ff2f7-8f46-4ac7-bfaf-9f645d937ef4.png)

🚩You can now see that there are a number of performance and usability improvements.

🚩When you interact with the story filter you can see an icon to indicate it is collapsible or expandable.
 
With Optimized View Mode, you can see that the drop down menu is much wider.

![7-53](https://user-images.githubusercontent.com/92877810/139122017-db72f3cd-9228-4f28-9ce3-55cff62daa03.png)

79. Deselect **All**

80. Select **Janet Bury**

81. Select **James Frank**

82. Click outside to collapse the story filter

![7-54](https://user-images.githubusercontent.com/92877810/139122018-96b0f7b3-4946-43f6-ae2e-026a6e243a2d.png)

83. Click the drop down icon to select the region

84. Deselect **EMEA North**

85. Deselect **EMEA South**

![7-55](https://user-images.githubusercontent.com/92877810/139122022-43488be2-7fb7-48d9-81e2-6edb631c1a46.png)

ℹ️With this new feature, you can undo any selections you made. 

86. Click **Edit**

87. Click **Undo**

![7-56](https://user-images.githubusercontent.com/92877810/139122025-47afde0c-e523-4874-b284-79ff4beb4e34.png)

⚠️**Quality Check!** Does your story look like this with all Regions selected?

![7-57](https://user-images.githubusercontent.com/92877810/139122026-867aff66-0dbd-4a3a-ba10-72de69736d29.png)

88. With Optimized View Mode, the hover over tooltip travels with your cursor as you move across the datapoint making it easier for the user to read.

![7-58](https://user-images.githubusercontent.com/92877810/139122028-d2cf6fa7-695b-49a3-8db1-9a03e3d8f166.png)

89. Right Click on the chart

![7-59](https://user-images.githubusercontent.com/92877810/139122029-51fdf340-cdc1-4f4c-9383-3dffce2d0501.png)

🚩**Notice!** With Optimized VIew Moode, the Actions menu is updated where you can see what are the filters and sorts that have been applied to this chart. Along with this you can also see other already available actions all in a single menu.

90. Click **Applied to Chart**

91. Click **Sort**

92. Click outside to close the Actions Menu

![7-60](https://user-images.githubusercontent.com/92877810/139122033-5f299f96-6e0c-41ca-af11-6d9191859749.png)

⚠️**Quality Check!** Does your story look like this? 

![7-61](https://user-images.githubusercontent.com/92877810/139122034-9777aa91-4ed9-468c-842c-8dd59e304d75.png)


