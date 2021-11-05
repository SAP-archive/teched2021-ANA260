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
