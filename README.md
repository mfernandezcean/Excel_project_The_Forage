
# **The FORAGE Project** 
[![descarga](https://github.com/mfernandezcean/Portfolio_Excel/assets/105746149/3d191430-d1cf-474e-84bc-2652b60c27e4)
](https://i.pinimg.com/originals/3c/2f/14/3c2f14aa90dcff8428907535df95dda8.jpg)

[KPMG virtual internship](https://www.theforage.com/modules/m7W4GMqeT3bh9Nb2c/S3uFvbDL49EA43ukg?ref=os5F6SHBM8o8xGJaD)

This projects is based on a simulated scenario created by KMPG in it's Virtual Internship.

Shortly, you work as a member of the Data Analyst's team of the firm with a **new client that is a mid-size company that sells bycicle and accesiories in Australia.**

The client is **looking** to **expand** to a ***new market*** and the goal is to assist them with recommendations, based on the analytical work, to **improve their marketing campaign**. 


This task has three steps:
 1. Data Quality Assessment 
 2. Data Insights & Model build 
 3. Visualising the results



# **1. DATA Quality**


### [Folder 1](https://github.com/mfernandezcean/Excel_project_The_Forage/tree/main/Worked_file/1.)
## ISSUES:
|  Table | Accuracy  |Completeness |Consistency |Currency|Relevancy|Validity
|--|--|--|--|--|--|--|
|**CustomerDemographic:**  | ***DateOfBirth*** Age information not provided| ***Job_title*** missing 506 rows (13% of total records)  ***Last_name*** missing 125 rows (6% of total records), ***Job_industry*** with 656 ‘n/a’ rows. (16.4% of total records) |***Gender*** is not consistent|***DateOfBirth*** record with an 1843 year of birth|***Deceased_indicator*** Information about deceased clients |***Default*** containing non- recognizable values ***Tenure*** information not clear or relevant 
|**CustomerAddres:**|***Address*** information all in one record|**NA**|***State*** is not consistent |**NA**|**NA**|***Property_valuation*** no clear reference of meaning for the value
|**Transactions:**|***Revenue*** information not provided|***Brand***, ***product_line***, ***product_class***, ***product_size*** missing 197 rows(1% of total transactions)|**NA**|**NA**|**NA**|***Transaction_date*** is for all 2017. Not only 3 months ***Product_first_sold_date*** format is not in date format ***List_price*** format not in currency |


## MEASURES TO BE TAKEN:
### For Accuracy:
**CustomerDeomographic**: 

 - **Issue**: column ***DateOfBirth*** information is not accurate. Age information is needed
 - **Mitigation**:  Creatin of an **'Age'** *column* in the data set 
 - **Recomendation**: Beyon gathering tyhe data of birtdate, also, at the same instance, collect or calculate the age of customers.

**CustomerAddress**:

 - **Issue**:  Address *column* has all the information in one field and this ***complicates*** the analysis.
 - **Mitigation**:  The *column* could be divided into two. One with the number and the other with the text
 - **Recomendation**: See this type of information as ***two separated*** instances.  
One is the number of the door and the other is the name of the street.  
The first is unique, the second could be repeated.

**Transactions**: 

 - **Issue**: No ***Revenue*** or ***Profit*** column provided
 - **Mitigation**:  Calculation of a ***Revenue*** column, using the *List_price* and *Standard_cost* columns
 - **Recommendation**: ***Configure*** in the system a calculation that gives the profit of ***every transaction***. 
---
### For Completeness:
**CustomerDeomographic**: 

 - **Issue**: *columns* ***Job_title, Last_name and Job_industry*** have missing values.
 - **Mitigation**:  Keep the ***analysis going forward*** taking note of the missing values
 - **Recomendation**:  In the *process of creating a new client*, generate a lock in the system that ***does not*** allow to finish the ***procedure*** with empty fields

**CustomerAddress**:

 - **Issue**:  -
 - **Mitigation**: -
 - **Recomendation**: -

**Transactions**: 

 - **Issue**: ***Brand, product_line, product_class, product_size*** missing rows
 - **Mitigation**:   Keep the ***analysis going forward*** taking note of the missing values
 - **Recommendation**: In the *process of creating a new client*, generate a lock in the system that ***does not*** allow to finish the ***procedure*** with empty fields
---
### For Consistency:
**CustomerDeomographic**: 

 - **Issue**: ***Gender*** is not consistent
 - **Mitigation**:  ***Unification*** of the classification of the dimension
 - **Recomendation**: ***Unification*** of the classification of the dimension

**CustomerAddress**:

 - **Issue**:  ***State*** is not consistent
 - **Mitigation**:***Unification*** of the classification of the dimension
 - **Recomendation**: ***Unification*** of the classification of the dimension

**Transactions**: 

 - **Issue**: -
 - **Mitigation**:  -
 - **Recommendation**:-

---

### For Currency:
**CustomerDeomographic**: 

 - **Issue**: ***DOB*** record with an 1843 year of birth
 - **Mitigation**:  ***Not taking in consideration*** the row. Is only one data record
 - **Recomendation**: Configure the year field with a logical **minimum** from where to choose

**CustomerAddress**:

 - **Issue**: -
 - **Mitigation**:-
 - **Recomendation**: -

**Transactions**: 

 - **Issue**: -
 - **Mitigation**:  -
 - **Recommendation**:-

---

### For Relevancy:
**CustomerDeomographic**: 

 - **Issue**: ***Deceased_indicator*** Information about deceased clients 
 - **Mitigation**:  ***Not taking in consideration*** the row. Is only two data record
 - **Recomendation**: If possible, ***separate*** the data from de Y and the N of the field. 
Don’t see possible use of deceased information. 


**CustomerAddress**:

 - **Issue**: -
 - **Mitigation**:-
 - **Recomendation**: -

**Transactions**: 

 - **Issue**: -
 - **Mitigation**:  -
 - **Recommendation**:-

---

### For Validity:
**CustomerDeomographic**: 

 - **Issue**: ***Default containing*** non- recognizable values **&**  ***Tenure*** information not clear or relevant 
 - **Mitigation**:  ***Default*** column deleted & Not taking in consideration for future calculations
 - **Recomendation**: If possible, **check** for columns with random characters. 

**CustomerAddress**:

 - **Issue**: ***Property_valuation*** no clear reference of meaning for the value
 - **Mitigation**: Not taking in consideration for future calculations
 - **Recomendation**: Summit a standard **scale** of the values.

**Transactions**: 

 - **Issue**: ***Transaction_date*** is for all 2017. Not only 3 months **&** ***Product_first_sold_date*** format is not in date format **&** ***List_price*** format not in currency
 - **Mitigation**:  Make the analysis with all the data available **&** Change the format to date ***&*** Change the format to currency
 - **Recommendation**:***Clarify*** the range needed to use for the analysis **&** In the data entry process, ***fix the format of the columns*** to avoid confusions
    
# **2. Data Insights & Model build**
### [Insights Presentation file](https://github.com/mfernandezcean/Excel_project_The_Forage/blob/main/Worked_file/2./Module_2_Template_slide_work.pptx)


 1. ***New South Wales Represents the 53% of the Total Revenue.*** 
Victoria 25% and Queensland 21%
 2. ***The Mass Customer segment represent the 50.1% of the Total Revenue*** High Net Worth 25.4% and Affluent Customer 24.3%
 3. ***Customers between 40-49 years tend to be more profitable than other ages.*** 50’s and 30’s combined reach a 34.16%
 4. ***By far, Standard Product is the most  Popular in the market.***    
 * Standard $ 8,138,860
 * Road $ 1,400,218
 * Touring $ 1,350,158
 5. ***54.8% of the Revenue comes from 3 industries:*** Manufacturing, Financial Services & Health
## Data Model:
![datamodel](https://github.com/mfernandezcean/Excel_project_The_Forage/assets/105746149/bc0927f4-bb50-46a1-8855-81447f964860)

