# Section 5 - Bookmarking and Sharing of a Story

⚠️This section builds on top of another section. If you did not complete the previous section, please select 
**“Section 4 – Theme and Style”** from the **“Public/TechEd”** folder and click **Copy To** your
directory. You will then be able to edit this story to complete the following exercise.

ℹ️**Objective:**  Collaborate with your colleagues by sharing your dashboard and setting up discussion points 
within SAP Analytics Cloud.

**Estimated Time:** 12 mins

**Exercise Description:** As a business analyst and content creator, you have finished creating your 
dashboard. You now need to share your dashboard with your colleagues. To help your colleagues be 
effective from the moment you share the dashboard, you can customize their view via bookmarks. Make sure 
to collect feedback from your colleagues about the dashboard before the executive meeting! 

**Key Features:**
- Create global and private bookmarks to create alternate views of the Story
- Share a Story with other users
- Learn how to create comments and @mentions
- Start a discussion with your colleges to track key decisions


⚠️**Disclaimer**
When completing exercises, some data values in the screenshots may not match what you see on your 
screen. This is because the dynamic time filters that were applied at the time the screenshots were taken is 
different from the current system date.

----------------------------------------------------------------------------------------------------------------------------------------

ℹ️In this section, we're going to learn how to bookmark states, share stories, add comments and have discussions with our colleagues.  

Bookmarks allow us to save the story in our preferred view. To showcase this, let's zoom in and analyze the performance of three Sales Managers.  
  
Compare your story with your screenshot, this is what it should look like at the start

![5-1](https://user-images.githubusercontent.com/92877810/138757055-f90cbea6-553c-4f0e-9c25-241b92a4280e.png)

🚩First, we're going to create a Story Filter for Sales Managers. 

1. Click **Tools**

2. Click **Story Filter/Prompt**

![5-2](https://user-images.githubusercontent.com/92877810/138757062-fd361b0d-0734-48ae-94e4-d5d6c28d9af0.png)

3. Click **Add**

4. Click **Dimensions**

5. Select **Sales Manager**

![5-3](https://user-images.githubusercontent.com/92877810/138757064-06015cd1-efc6-4b7f-a991-eafc736815a5.png)
  
🚩We want the ability to filter by all the Sales Managers. 

6. Click **All Members**

7. Click **OK**

🚩Press **Ctrl + S** to save the story

![5-4](https://user-images.githubusercontent.com/92877810/138757067-5efa304e-00d0-4d7e-9f35-bb9f6f6fe6da.png)
  
🚩Now that we've created the filters. We're going to be interacting with them. This can be done in **View Mode**. 

8. To enter view mode. Click **View**

![5-5](https://user-images.githubusercontent.com/92877810/138757070-50ed3c06-9d18-4ed7-84ea-498c4b14cd77.png)

🚩Now that we're in View mode, let's change the state of the story. Remember, we wanted to analyze the performance of specific sales managers? 

9. Click **Sales Manager**

10. Deselect **All**

11. Select three managers - **Janet Bury, Gary Dumin and James Frank**

![5-6](https://user-images.githubusercontent.com/92877810/138757074-a4c76968-9949-4b4a-8677-3b8207aac1e4.png)
  
🚩To gain better insights, we can narrow down the region and see what the performance for these Sales Managers was in the specified regions we're interested in.  

12. Click **Region**

13. Deselect **All**

14. Select **MEE**

15. Select **NA**

16. Click outside the **Input Control** to Collapse

![5-7](https://user-images.githubusercontent.com/92877810/138757075-0456bbc8-b659-40d9-af73-2413519486ac.png)

🚩Let's narrow down the Product filter and see if performance is affected.  

17. Click **Product**

18. Expand **All**

19. Deselect **Accessories**

20. Click outside the **Input Control** to Collapse

![5-8](https://user-images.githubusercontent.com/92877810/138757077-64b0c205-80de-49a9-8072-8dd18e6707ed.png)

🚩We've seen the performance based on 
Gross Margin, but what about Sales Revenue? Are the managers performing differently based on that measure? Let's find out.  

21. Click **Sales Revenue** in the **Measure Input Control**

![5-9](https://user-images.githubusercontent.com/92877810/138757079-5899ddcd-d6e8-4df1-9b94-bc21526c1079.png)

⚠️Quality Check! Does your dashboard look like this? 

![5-10](https://user-images.githubusercontent.com/92877810/138757081-62118470-8dba-4ebd-9db8-3facd37cac1f.png)

🚩Now that we have our story in a modified state, let's bookmark it so the state can be recalled later.  

22. Click **Bookmark**

23. Click **Bookmark Current State**

![5-11](https://user-images.githubusercontent.com/92877810/138757084-d9ed4052-9bd6-4065-a16b-4699b3fa192d.png)

ℹ️Welcome to **Bookmarking**!  
Bookmarking allows content consumers to have a customized view saved so that they can simply consume the saved state later. 
  
Designers can create global bookmarks that are visible to anyone with access to the story. When sharing a story, a designer can also assign a default global bookmark.  
 
Viewers also can create private bookmarks that are only visible to them or if they choose to share with others then they are visible to the shared group as well.  

![5-12](https://user-images.githubusercontent.com/92877810/138757087-32e852a8-14e8-48fc-a3df-b26da772472d.png)

24. Let's name our bookmark **Overview for Janet, Gary, and James**

25. Select **Global** so this bookmark can be visible to any team members we choose to collaborate with.  
 
26. Click Set as **new default**

27. Click **Save**

![5-13](https://user-images.githubusercontent.com/92877810/138757089-5bc006a5-c9df-4c57-af03-7bb3a1139a68.png)

ℹ️Let's share this story with our colleague Tony and see if he agrees with our analysis. 

28. Click **File**

29. Click **Share**

![5-14](https://user-images.githubusercontent.com/92877810/138757092-f6605fbf-ba2f-428b-946e-def10631a268.png)

30. Type in **Tony**

31. Select **Tony**

![5-15](https://user-images.githubusercontent.com/92877810/138757094-b143e17d-9d35-4df8-838e-9223fc96da1f.png)

🚩We want Tony to see the story in the bookmarked state by default. 

32. Select **Apply Global Bookmark Default**

33. Expand **Bookmark**

34. Select **Overview for Janet, Gary, and James**

![5-16](https://user-images.githubusercontent.com/92877810/138757098-5d060243-7326-46fc-b264-eec643ad83c4.png)

🚩These selections will apply the bookmarked state to the story as soon as Tony opens it. Allowing him to view the insights on Sales 
Manager performance we were looking at

35. Click **Share**

36. Click **Close**

![5-17](https://user-images.githubusercontent.com/92877810/138757100-1ea89201-8385-403e-a5c7-21d1ff99eaf5.png)

⚠️Take a minute to save your work by using the Save Icon or pressing **Ctrl + S**. 

🚩Now that we have created and shared the bookmark, we can return to this state at any time. Let's revert the changes and go back to our original Overview Dashboard. 

37. Click **Sales Manager** Story Filter

38. Select **All**

39. Click Outside the Sales Manager Drop Down Menu

![5-18](https://user-images.githubusercontent.com/92877810/138757101-66578184-6f2e-444d-bc61-2fd8933aba83.png)

40. Click **Product Page Filter**

41. Click **All**

42. Click Outside the Input Control to Collapse

![5-19](https://user-images.githubusercontent.com/92877810/138757105-d6f8bbfb-7410-413c-946d-e2afd7756fa7.png)

43. Click **Region**

44. Select **All** Regions

45. Click Outside the Input Control to Collapse

🚩We're back to the original state.  

![5-20](https://user-images.githubusercontent.com/92877810/138757107-22ea44de-1d98-44ed-9baf-04648247bb6e.png)

🚩We now want to analyze the performance of all our Sales Managers in the EMEA North and EMEA South Regions. Let's create this filter and bookmark it for our personal use so we can refer to it later. 

46. Click **Region Page Filter**

47. Deselect **All**

48. Select **EMEA North** and **EMEA South**

49. Click Outside the Input Control to Collapse

![5-21](https://user-images.githubusercontent.com/92877810/138759517-d437c254-8140-41f5-9b5f-0e3e0939585e.png)

50. Click **Bookmark**

51. Click **Bookmark Current State**

![5-22](https://user-images.githubusercontent.com/92877810/138759523-eae6ff0a-ee97-4064-98e1-944b060f6b17.png)

52. Name the Bookmark **EMEA** Overview

ℹ️This time we're going to make it a personal bookmark for use by ourselves only. 

53. Click **Personal**

54. Click **Save**

![5-23](https://user-images.githubusercontent.com/92877810/138759525-954d29ca-9ed5-456c-90ba-f125963b2435.png)

🚩Now that we have a bookmark, we can easily come back to this state. Let's go back to our global bookmark and notify our colleague Tony by leaving him a comment

55. Click **Bookmark**

56. Expand **Open Saved Bookmarks**

57. Click **Overview for Janet, Gary, and James**

![5-24](https://user-images.githubusercontent.com/92877810/138759526-6b1e4d7f-54b4-4cd2-882a-59f5d1905a08.png)

⚠️Quality Check! Let's make sure we're back in the state we had bookmarked. 

![5-25](https://user-images.githubusercontent.com/92877810/138759530-40c87eb0-0e20-4243-9c4b-3a618636d40b.png)

🚩Once we're back in the bookmarked state, we can add a comment. 

58. Click **Edit** (if not already in edit mode)

59. Expand **Overview**

60. Click **Comment**

![5-26](https://user-images.githubusercontent.com/92877810/138759533-bbc32cd3-df40-4a72-b799-933f3551b5b9.png)

61. Search for Tony by typing "@" before Tony

62. Once the desired person shows up, click their name so they can be notified

![5-27](https://user-images.githubusercontent.com/92877810/138759536-7bc53c4c-e0cd-4d2f-813c-5c14f4b575d1.png)

63. Type **@Tony Please see the Overview page here**

64. Click **Add Comment**

![5-28](https://user-images.githubusercontent.com/92877810/138759538-34ade29d-b4dd-4ede-8771-be112817ec48.png)

🚩Once the comment is placed, you can interact with it further. For example, you 
can click the like icon. This can be done for your own or someone else comment and they will see this interaction. 

65. Hover over the comment and Click the **Like** icon

66. Click **Exit** to close the comment dialogue

![5-29](https://user-images.githubusercontent.com/92877810/138759543-d0228aec-8c5f-42c8-8c81-e7c40836a81a.png)

⚠️Quality Check! Does your dashboard look like this?  
  
This is also a good time to Save your Story
  
🚩Press **Ctrl + S** to save your story

![5-30](https://user-images.githubusercontent.com/92877810/138759547-3e60cf8a-3923-4f24-b48a-d46013f86fbf.png)

🚩SAP Analytics Cloud allows users to collaborate on stories. This can be done via discussions.  

67. Click **Collaborate**

68. Click **New Discussion**

![5-31](https://user-images.githubusercontent.com/92877810/138759640-00b91aa0-4f98-475c-8ed4-a0900855bddb.png)

ℹ️Welcome to the Discussion Panel! This is where we can collaborate with our colleagues and discuss the story. 
  
Let's start by inviting someone to the discussion. 

69. Click **Invite Participants**

![5-32](https://user-images.githubusercontent.com/92877810/138759643-86aed1f9-258f-42c2-a959-ba1f970a0922.png)

70. Search for **Tony**

71. Select **Tony**

72. Click **OK**

![5-33](https://user-images.githubusercontent.com/92877810/138759644-415b2277-bb8c-4c65-a6ef-49d09cc13888.png)

🚩In the discussion panel, we're going to point Tony towards a specific story, and we're going to link it, so he knows which story we're talking about. 

73. Write Tony a message:  i.e. **Hey Tony, this is the overview page for our company's finances**

74. Press **ENTER** or click the **Send** icon to send

![5-34](https://user-images.githubusercontent.com/92877810/138759646-6c350819-46cd-4613-90a2-458f7ab68d1d.png)

🚩Now let's link the story so Tony knows what we're talking about. 

75. Click **New**

76. Select **Link Story** and the story we have open will be linked

![5-35](https://user-images.githubusercontent.com/92877810/138759648-f32843cd-1973-4add-a70d-41a7f506cc7a.png)

⚠️Quality Check! This is what your screen should look like once you’ve linked the story.  
  
This is the end of the section! You’ve learned how to create global and personal bookmarks, how to share stories in bookmarked states, comment on pages (and tag people in comments) and start discussions. 
  
Make sure to Save your story before moving on to the next section.  

![5-36](https://user-images.githubusercontent.com/92877810/138759650-a819cf8d-c062-4f20-9bb5-8b55af983ed1.png)

<br><br>

## Summary

**You have completed the entire Collaboration and Bookmarking section!**

**You are now able to:**
- Create global and private bookmarks to create alternate views of the Story
- Share a Story with other users
- Create comments and @mentions
- Start a discussion with your colleges to track key decisions


