
# Aryans_Store-Dashboard

### Dashboard Link : https://drive.google.com/drive/folders/15ObspmhTP_IQKSfQAhtOGmZ5Cue7Ivc8?usp=sharing

## Problem Statement

This dashboard helps the Sales Team understand their perforemence better. It helps the Aryan General Store's decision maker to know the perforemence of the store throughout the year categorized as monthly and quarterly profits, Highlighting the Most profitable to the losses incured.

this data highlights the most sold products throughout the year divided by categories and sub categories. Along with information about which product hit its peak in which month and which was its bottom period giving a clear insight on distributing the time and resources accordingly.
This data is a Exceptionaly benefitial for the sales team to make sales related decision's and targets and to prepare suitable measures to reach them.

### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a xlsx file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column Amount", "column category" & "column month" options.
- Step 3 : Also load another dataset into power BI dekstop, an xlsx file containing data from sales of sub category "column subcategory" & "column profits" & "column order id"
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : for calculating the amount of profit earned every month both the column category and profit were taken in use.
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Since the data contains various months worth of data, thus in order to distinguish the monthly progress, a new visual was added using the three ellipses in the visualizations pane in report view.
- Step 8 : Visual filters (Barchart) were added for more detailed and easy understanding.
- step 9  : personel customization was done to diffrentiate the months of profits to the months of losses.

[SNAP] ![Screenshot 2024-08-12 232904](https://github.com/user-attachments/assets/8f9ced61-b2ae-4c68-b05e-88fa3de76f51)


- Step 10 : two new visuals was added to the canvas, one representing the most profitable stores by state & other representing average order value to know the economic order quantity of customers.
  used & null values were unselected for consideration into average calculation.
           
           Although, by default, while calculating average, blank values are ignored.(thought there were a very few blaank values that didn't affected the entireity of the data)
- Step 11 : A pie chart was also added to the report design area representing the number of customers on the basis of mode of payment. While creating this visual, field named "mode of payment" was added to the Legends bucket.

[SNAP] ![Screenshot 2024-08-12 233321](https://github.com/user-attachments/assets/b697eb36-e923-407d-9691-650a594661c0)


- step 12 : A line chart was added to see a specific category product perforemence throughout the year giving insights on its peak & bottom sales.

[SNAP] ![Screenshot 2024-08-12 233401](https://github.com/user-attachments/assets/d3df31fb-820f-4b0a-84e0-ac65bbd141af)


- step 13 : Small tabs were added to show the "yearly profit" & "sum of quantity" & "sum Of Amount".
[SNAP] ![Screenshot 2024-08-12 232923](https://github.com/user-attachments/assets/83cba924-a84a-4774-8d5a-d704c2ae9990)  ![Screenshot 2024-08-12 232917](https://github.com/user-attachments/assets/00cf67a6-b613-4a53-bd4e-e27d38ba2dcf)
 ![Screenshot 2024-08-12 232910](https://github.com/user-attachments/assets/b24a710f-43a1-4c46-8173-d34b83cdc9ad)





- step 14 : to top this data State wise filteration was added so that it can be used by all the branches realted to there own stores.
[SNAP]![Screenshot 2024-08-12 233711](https://github.com/user-attachments/assets/9035453a-8825-475f-8038-821fbc3f48cf)



- step 15 : at last (slicers) were added to give it a quarterly based breakdown for more easy to iunderstand and to have a clean look.

[SNAP]![Screenshot 2024-08-12 233822](https://github.com/user-attachments/assets/45492d2a-5d89-430a-b660-31d5f964fb30)

  
In our dataset, Some parameters were assigned with a unique order id, those are assigned uniquely different from each other.

- Step 16 : In the report view, under the insert tab, one text boxes was added to the canvas, in this text box name of the store was mentioned 
- Step 17 : Calculated column was created in which, Average order value was mentioned for a better understanding for future estimates.

for creating new column following DAX expression was written;
       
        Aerage order value=  [Total Amount] * [Total Quantity]
        
Snap of new calculated column ,

[Snap]![Screenshot 2024-08-12 182730](https://github.com/user-attachments/assets/83d5121e-08ba-431f-9489-0d5eb71163a5)



        
- Step 18 : A small box was used to describe the average order value.

[Snap]![Screenshot 2024-08-12 232929](https://github.com/user-attachments/assets/986dfece-1903-493c-8856-dfe4d93725e1)
 
 - Step 18 : The report was then published to Power BI Service.
 [Link]https://drive.google.com/file/d/1JID6Z0gs8n2NwPUdBtxeZlhEwgXLiTJf/view?usp=sharing

# Snapshot of Dashboard (Power BI Service)

[Snap] ![Screenshot 2024-08-12 234142](https://github.com/user-attachments/assets/21ef127d-986b-494b-a40f-2c58d5bb6e1c)





 # Report Snapshot (Power BI DESKTOP)


# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] A trend of decrease in profits is clear visible from the month january to the month of december.
Quater 1 being the highest with: 
   
   sum of gross sales() and gorss profits  = sales(161000) profits(26000)
   with stationary items being the higest category in sales.


following up with quarter 2 which has shown a major down slope even making losses
   sum of gross sales() and gorss profits  = sales(87000) profits(882)

Quareter 3 having
sum of gross sales() and gorss profits  = sales(72000) Loss(1469)
   
Quarter 4 regaining the sales volume and profit with
sum of gross sales() and gorss profits  = sales(118000) profits(12000)
           
           thus conclusion can be made that sales are highest in the initial months of the year the reason could be the sense of buying new products during the start of the year among the customers.

### [2] Higest Sellings by Category in %

    a) clothing (62.62%)
    b) Electronics(20.55%)
    c) Furniture(16.83%)
    
  
  These ratings will change if different visual filters will be applied.  
  
  ### [3] Most profitable stores (state wise)
  
      a) Madhyapradesh
      b) Maharashtra
      c) Uttarpradesh
Profits will change if monthly visual filter will be applied.

 ### [4] Some other insights
 
###### link(piechart)
 
 1.1)  More then 81% of the payments are done in cash & kind indicating a short period of conversion cycle which is a good indicater 
 
 1.2) 10.9% is done with Credit card, and
 
 1.3) 8% is done through EMI options.
 
         thus, the stores are able to maintain a good liquidity ratio.
 
 ### [conclusion]
 * With the help of this dashboard major insights can be easliy understandable by the sales department and future action can be more precise and new aims could be developed with better targets.        

# Aryan Store- ... oard.md.txt
Displaying # Aryans.store-Dashboard.md.txt.

