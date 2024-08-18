#  Market survey insight for food & Beverage industry .

### Dashboard Link : 

## Problem Statement

CodeX is a German beverage company that is aiming to make its mark in the Indian market. A few months ago, they launched their energy drink in 10 cities in India.

Their Marketing team is responsible for increasing brand awareness, market share, and product development. They conducted a survey in those 10 cities and received results from 10k respondents. Aa  a marketing data analyst im  tasked to convert these survey results to meaningful insights which the team can use to drive actions.  

### Steps followed 

- Step 1 : Load data into Power query , dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so we need to select "column profiling based on entire dataset".
- Step 4 : Created a dimension table for brands  to normalize data & merged brand_id to fact survey table .



           
- Step 8 :DAX measures created for comprehensive & robust analysis and to create necessary kpi's .
           
           -Female respondents = CALCULATE([Total respondents],dim_repondents[Gender]="Female").
           -Male respondents = CALCULATE([Total respondents],dim_repondents[Gender]="Male"). 
           -Respondents % = DIVIDE([Total respondents],CALCULATE([Total respondents],ALL('fact_survey_responses')))
           -Total respondents = COUNTROWS(fact_survey_responses)
          
          

- Step 9 : 3 report page created Homepage , Habitual_insight , brand perception .

- Step 11 : Answering business questions & provide Recommendations .



## Business request 1 : Who prefers energy drink more? (male/female/non-binary?),  Which age group prefers energy drinks more? ,Which type of marketing reaches the most Youth (15-30)?


![Screenshot 2024-05-25 150114](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/2a73d5e5-7989-4271-bdd2-f6321aad1b1c)
![Screenshot 2024-05-25 140610](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/78e5a0b6-c805-4223-93b2-1407a80eac35)

![Screenshot 2024-05-30 210255](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/fc00cf78-ac7c-4c34-959c-066b6c00f6b5)
![Screenshot 2024-05-25 141927](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/d24ab2e4-cd62-4c41-973e-9e278c65e200)

-  Diwali have the upper edge when it comes to 33% & cashback promo as it generates high isu%  ; 
- Even though when it comes to promotion based on product pricing sankranti clearly has the upper edge as  low to moderate pricing product has significant growth in sankranti due to its promo offer to certain products  ! ;
- Diwali also as high IR as it offers more 50% off promo in low price section on contrary 
   sankranti offers more BOGOF promo one of the reasons for its high ISU %  ;
- Based on IR% Diwali is Successful and based on ISU% Sankranti is heavy Successful.
- Sankranti is successful when it comes to balance between IR% and ISU% .
      

## Business request 2 : What are the preferred ingredients of energy drinks among respondents?, What packaging preferences do respondents have for energy drinks?
![Screenshot 2024-05-26 203133](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/28e9ca64-4046-4af3-9b64-ff86e7bd82b3)


- Cancelation trend going upwards since apr and making a constant impact till october 
- At the other end it clearly observed that avg daily rate has a upward trend till Aug .
- Avg daily rate has a key impact driving canceled booking over time !

## Business request 3 : Who are the current market leaders?  What are the primary reasons consumers prefer those brands over ours?
 
![Screenshot 2024-05-26 233432](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/f5fcef02-bbd1-47fa-9df4-3be07bb93dfc)
![Screenshot 2024-05-29 200941](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/ef8830e2-f30f-438e-8ae2-8f44f384446c)
![Screenshot 2024-05-29 201034](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/30dcadad-f5dc-4d23-a24b-2abdd5ae3148)
![Screenshot 2024-05-30 202142](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/81c1624a-148c-41e4-b0e5-9a7a57ba2d15)


- Almost 97% of Incremental revenue is generated from cashback & BOGOF promo !
 - cashback promo is Successful in Diwali campaign & BOGOF is Successful in Sankranti festivel .
 - 25% promo is a failed promo when it comes to revenue &  sold quantity !

 
 ## Business request 4 : Which marketing channel can be used to reach more customers ?How effective are different marketing strategies and channels in reaching our customers? 
