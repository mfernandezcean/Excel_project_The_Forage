# **The FORAGE Project (KPMG Australia)** 
[![descarga](https://github.com/mfernandezcean/Portfolio_Excel/assets/105746149/3d191430-d1cf-474e-84bc-2652b60c27e4)
](https://i.pinimg.com/originals/3c/2f/14/3c2f14aa90dcff8428907535df95dda8.jpg)

[KPMG virtual internship](https://www.theforage.com/modules/m7W4GMqeT3bh9Nb2c/S3uFvbDL49EA43ukg?ref=os5F6SHBM8o8xGJaD)

This projects is based on a simulated scenario created by KMPG in it's Virtual Internship.

Shortly, you work as a member of the Data Analysys team of the firm with a *new client that is a mid-siza company that sells bycicle and accesiories in Australia.*

The client is **looking** to **expand** to a new market and the goal is to assist them with recomendations, based on the analytical work, to **improvie their marketing campaing**. 


This task has three steps:
 1. Data quiality asistmen 
 2. Data model build 
 3. Vizualise the results

## **1. DATA QUIALITY**

[Video](https://www.loom.com/looms/videos/KPMGForage-fc15f18018894c15bedfa4ab377e0f37)

![Picture1](https://github.com/mfernandezcean/Excel_project_The_Forage/assets/105746149/da18c294-bf05-458a-ba6d-1c7d712512ec)


## **1. DATA QUIALITY**
[Video](https://www.loom.com/looms/videos/KPMGForage-fc15f18018894c15bedfa4ab377e0f37)

|  Table | Accuracy  |Completeness |Consistency |Currency|Relevancy|Validity
|--|--|--|--|--|--|--|
|**CustomerDemographic:**  | ***DateOfBirth*** Age information not provided| ***Job_title*** missing 506 rows (13% of total records) ***Last_name*** missing 125 rows (6% of total records), ***Job_industry*** with 656 ‘n/a’ rows. (16.4% of total records) |***Gender*** is not consistent|***DateOfBirth*** record with an 1843 year of birth|***Deceased_indicator*** Information about deceased clients |***Default*** containing non- recognizable values ***Tenure*** information not clear or relevant 
|**CustomerAddres**|***Address*** information all in one record|**NA**|***State*** is not consistent |**NA**|**NA**|***Property_valuation*** no clear reference of meaning for the value
|**Transactions**|***Revenue*** information not provided|***Brand***, ***product_line***, ***product_class***, ***product_size*** missing 197 rows(1% of total transactions)|**NA**|**NA**|**NA**|***Transaction_date*** is for all 2017. Not only 3 months ***Product_first_sold_date*** format is not in date format ***List_price*** format not in currency |
