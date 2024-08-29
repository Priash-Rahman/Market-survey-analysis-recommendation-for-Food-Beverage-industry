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

![Screenshot 2024-08-29 202537](https://github.com/user-attachments/assets/e1ebea3e-3fbe-4ed1-b36f-c35a7c7c872a)

- 60% of our  customers are male , 70% of customers are youth age ranging 15-30 combinedly, though 55% alone  is19-30.
- Online & TV commercials have huge impact on youth(15-30), out of 40% respondents 35% are impacted by online ads & of 27% respondents 18% are impacting youth (15-30).

      

## Business request 2 : What are the preferred ingredients of energy drinks among respondents?, What packaging preferences do respondents have for energy drinks?
![Screenshot 2024-08-29 210407](https://github.com/user-attachments/assets/fa2ed739-a8eb-4687-984c-0ef7084ba722)


- Caffeine , vitamins are the most preferred compounds among respondents comprising of 65% 
- Compact-portable cans & innovative bottle design are most preferred by respondents.           

## Business request 3 : Who are the current market leaders?  What are the primary reasons consumers prefer those brands over ours?    (Competition analysis)



- Almost 97% of Incremental revenue is generated from cashback & BOGOF promo !
 - cashback promo is Successful in Diwali campaign & BOGOF is Successful in Sankranti festivel .
 - 25% promo is a failed promo when it comes to revenue &  sold quantity !

 
 ## Business request 4 : Which marketing channel can be used to reach more customers ?How effective are different marketing strategies and channels in reaching our customers? 
