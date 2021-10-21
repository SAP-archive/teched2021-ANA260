# Section 3 - Geo Maps, Thresholds, and Variance

Welcome to the **Geo Maps, Thresholds and Variance** section! We will also go into greater detail on the analytic capabilities available to story creators with geo maps and geo-enriched data in our **Section 8 - Geo Visualizations Deep Dive**. 
 
Exercise check! Does your dashboard look like this screenshot? 

![3-1](https://user-images.githubusercontent.com/92877810/138260047-5b7838cf-581e-4a86-a6a0-8a4c4f0b9425.png)

Let us start by adding some geographical information into our dashboard. 

1. Click **Insert**

2. Click **Geo Map**

![3-2](https://user-images.githubusercontent.com/92877810/138260049-7ffbb9bb-7abd-425d-9069-39ca7a288e74.png)

Quality check! Does a geo map appear at the bottom right of your dashboard like this screenshot? Does the Builder panel open with your geo map selected? 

![3-3](https://user-images.githubusercontent.com/92877810/138260051-4ecc4fda-699e-4271-a5ff-d23e9cdd07db.png)

Geo visualizations consist of one or multiple layers which can be sourced from different data sets. For our purposes, we will be using a bubble layer to individually represent measure values at store coordinates. 

3. Click **+ Add Layer**

![3-4](https://user-images.githubusercontent.com/92877810/138260052-c4f2d99b-7b7b-4a6a-89be-93ea722436c0.png)

We are going to be using a secondary model in this exercise. SAP Analytics Cloud supports using multiple models in a dashboard to best represent your story. Let us swap to our shipping model so we can display average delivery times by country in our geo map. 

4. Click **Select Model**

![3-5](https://user-images.githubusercontent.com/92877810/138260053-507e3619-6d00-463e-8ecd-7e5c20722133.png)

5. Click **Select Other Model...**

![3-6](https://user-images.githubusercontent.com/92877810/138260055-4d81c8c7-1758-47e1-ae54-fb351b037842.png)

6. Click **Public**

![3-7](https://user-images.githubusercontent.com/92877810/138260056-c6ee6d2f-e9aa-4cdf-a3f1-03b33be74531.png)

7. Click **TechEd 2021**

![3-8](https://user-images.githubusercontent.com/92877810/138260057-7a796520-f0ec-437a-ae32-592a4231b91f.png)

8. Click **ANA260_SHIPPING_INFO**

![3-9](https://user-images.githubusercontent.com/92877810/138260058-8d7a5e9c-1dd6-4b6e-9af3-35f79e0a9521.png)

9. Click **Add Location Dimension**

![3-10](https://user-images.githubusercontent.com/92877810/138260059-f48c47ca-65b7-496a-96c5-c35140cc718b.png)

The dimension displayed in Location Dimension is a geo-enriched dimension that can be built in your dataset from location names or latitude/longitude coordinates. 

10. Click **StoreLocation**

![3-11](https://user-images.githubusercontent.com/92877810/138260785-182f29d8-45fd-47c4-9432-bd954c358bf2.png)

Quality Check! Does your Geo Map populate with stores like this screenshot? 

Let us color our bubbles based on average delivery time so we can easily see which locations are taking longer to receive deliveries.

![3-12](https://user-images.githubusercontent.com/92877810/138260788-bef29639-0489-4d12-b9ea-f5a81f327ee0.png)

11. Click **+ Add Measure/Dimension**

![3-13](https://user-images.githubusercontent.com/92877810/138260790-0ca830f6-d835-4991-8709-b0825490e69c.png)

Let us select average delivery time to color code our bubbles so we can identify which stores are receiving deliveries slower. 

12. Click **Avg Delivery Time**

![3-14](https://user-images.githubusercontent.com/92877810/138260791-1d7027a3-9b67-4b4a-ae3e-f59d841bcc3c.png)

Quality check! Does your geo map look like this screenshot? Next, we will look at using a different layer type to represent our data. 

![3-15](https://user-images.githubusercontent.com/92877810/138260792-abab03c4-3b01-47dd-b6d0-f5d2117228ea.png)

There are other layers applicable to our 
Geo Map. Let us look at average delivery time aggregated based on location rather on an individual store level. We can do this by choosing to add a choropleth layer. We will go into further detail on the other layer types available in SAP Analytics Cloud in our **Section 8 - Geo Visualizations Deep Dive** section. 

13. Click **Expand** for **Layer Type**

14. Click **Chloropleth/ Drill Layer**

![3-16](https://user-images.githubusercontent.com/92877810/138260793-5ea01bb8-cf4f-4d2e-be62-6f9ee2433ee1.png)

A choropleth layer aggregates values in the Geo Map, making it easier for a user to discover outliers and trends. As we can see in the geo visualization, Spain appears to have higher than average delivery times on orders. Let’s drill down on this layer to understand the data. 

15. Click on **Spain**

![3-17](https://user-images.githubusercontent.com/92877810/138260795-64a9371f-0cce-427e-a879-06fe6c42cdf0.png)

When we click on Spain, we get a context menu with options to Drill down or up on the hierarchy level as well as filter on or exclude Spain's data from the geo map. We want to look at regional average delivery times in Spain so let us drill down on this hierarchy. 

16. Click **Drill Down**

![3-18](https://user-images.githubusercontent.com/92877810/138260796-bbf023d8-7f53-4765-9095-93630ef6d8d0.png)

From drilling down on our country layer, we are now able to see the distribution of average delivery times in the regions of Spain. It appears only one region is doing poorly and may require further business action. Let’s return to our country layer. 

17. Click **Drill Filter**

18. Click **Remove**

![3-19](https://user-images.githubusercontent.com/92877810/138260798-22695941-29db-43fa-a263-fb16718c2dcc.png)

Quality check! Does your geo map now look like this screenshot? 

![3-20](https://user-images.githubusercontent.com/92877810/138260799-1b3045eb-3ab4-407e-bf96-f5b28ced95bd.png)

