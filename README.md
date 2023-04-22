# Project-1---Revisited
---
## Top Three Features for Linear Regression Model for Determining Price
---
1. Outlet Type is the most important feature if the outlet type = grocery store it has a -1500 impact on the outlet sales.
2. Outlet Size is the second most important feature, those with a High size receiving 500+ to their total sales.
3. Item Visibility is the third most important feature with a negative coefficient of of almost 500.
![Lin_reg Coeff](https://user-images.githubusercontent.com/49537432/232902015-3cf0a803-dd76-4596-8a30-9c1d1b966327.png)

## Top Three Features for Determing Sales Total with a Random Forest Model
---
1. Item MRP accounted for roughly 40% of the total sales determination. 
2. Outlet Type = grocery store accounted slightly more than 20% of the final total sales.
3. Item visibility accounted for slightly more than 10% of the final total sales.
![rf_importance](https://user-images.githubusercontent.com/49537432/232902154-fd9d783e-012f-425f-853f-d652a9b65d4a.png)

Feature Importance Bar Graph:

Outlet_Type_Supermarket Type3
Outlet_Size_High
Item_Type_seafood
Permutation Importance Bar Graph:

Item_MRP
Outlet_Type_Supermarket Type3
Outlet Type Grocery Store
The two graphs identified different features as being importance, the only feature they have in common being Outlet_Type_Supermarket Type3 though in different positions of importance.

![image](https://user-images.githubusercontent.com/49537432/233791564-a4c48678-2e53-4942-a166-087fbb182895.png)

## Permutation Bar Graph Analysis
---

1. Item MRP - When Item MRP is of a higher value the overall sales of the store also increases. 
2. Outlet_Type_Supermarket Type3 -When this feature has a higher value sales increase.
3. Outlet Type Grocery Store - When the grocery store is type 3 the 
![image](https://user-images.githubusercontent.com/49537432/233791677-0629e2b2-418b-48db-82ed-7c91a9153a03.png)

## Local Explanations
---

The first example data I choose was the sample with the highest MRP as that was the most impactful feature according to permutation analysis. Second, I choose outlet establishment year to test if more recent openings produced better results

###
---
MRP: 
![mrp force](https://user-images.githubusercontent.com/49537432/233804058-bc3f63aa-0e6f-4a18-9854-7db25fc36408.PNG)
Feature impact on model according to force plot
1. Item_MRP had the greatest impact increasing the final score by the most overall ~ 1800
2. Outlet_Type_Supermarket Type3 = 0 had the most negative impact on final score
3. Outlet_Size = 0 had a negative impact on the model decreasing the predicted score by ~300

![mrp lime](https://user-images.githubusercontent.com/49537432/233804060-ce2ee8fb-45c0-4e02-9233-cae0033383b5.PNG)
Feature impact on model according to force plot
1. Item_MRP had the greatest impact increasing the final score by the most overall ~ 1800
2. Outlet_Type_Supermarket Type3 = 0 had the most negative impact on final score
3. Outlet_Size = 0 had a negative impact on the model decreasing the predicted score by ~300

Established Year:
![year established force](https://user-images.githubusercontent.com/49537432/233804077-14956408-28ac-47fd-9091-08902c4d4b40.PNG)
Feature impact on model according to force plot
1. Item_MRP = 178.3 had the largest impact increasing the predicted total sales by ~ 500
2. The high Outlet_Establishment_Year = 2009 had the second largest positive impact increasing the predicted sales by ~200
3. Outlet_Type_Supermarker Type2= 1 had the largest negative impact decreasing the score by ~400

![year established lime](https://user-images.githubusercontent.com/49537432/233804088-f6ec1568-c4e1-4951-b644-1e84886b0f1a.PNG)

Feature impact on model according to limee
1. Outlet_Type_Grocery had the highest impact increasing the predicted value by ~2200
2. Outlet_Type_Supermarket had the highest negative impact decreasing predicted value by ~800
3. Item MRP > 143.61 had the second largest impact increasing the score by ~550
