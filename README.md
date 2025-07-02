# HealthSector_BI
A Health Sector Report analyzing various Chronic diseases / Non-communicable diseases (NCDs) from 2019 to 2021 thourgh various metrics.

# Chronic diseases / Non-communicable diseases (NCDs) Analysis

## Steps followed : 

- Getting Data from Kaggle for various (NCDs) 
         "Healthcare_Dataset " is a Excel Worksheet file.

## Meta Data :

      Sheet1- Patient Data
              
Patieint ID
Name
Age
Gender
Blood Type
Medical Condition
Date of Admission
Doctor
Hospital
Insurance Provider
Billing Amount
Room Number
Admission Type
Discharge Date
Medication
Test Results
Insured Amount
	
	Sheet2- Trustee 
Hospital Code	
Hospital Name
Trustee Name

## Load in Power-Bi

1.Get Rid of any Blank, Null & Duplicate Patient Id's
         
2.Create Calendar table for calculating
Date
Month_No
Year
Month_Name
Date_of_Month
Month + Year
Start_Of_Month
End_Of_Month
Start_Of_Year
End_Of_Year
Quater
Start_Of_Quater
 
Create a relationship of one to many (1->*) from Calendar -> Patient Data.

3. Create Calculated columns for measuring 

Age_Groupp
Treatment Time(Days)
Cost_to_Customer

4.Creating a Measure table to hold Dax Queries

%Emergency_Cases_of_Total
%Urgent_Cases_of_Total
%Elective_Cases_of_Total
%_avg_ot_insurance_amount_covered
Age_Gourp
BloodType_Count
Cost_to_Customer
Count_Of_Cases
Count_Of_Cases(color)
Count_Of_Cases(Male)
Elective_Cases
Emergency_Cases
Expenses
Highlighting Meassure
Highlighting_Meassure_Casetype
Max_Casetype_per_Condition
Max_Condition_per_age_group
MaxDate
MinDate
Urgent_Cases

        
* Using Matrix, Table, Bar-Graph, Line-Chart, Tooltips, Letter & Pie-Chart to Analyze all Factors for Overall and Particular Higher Medical cases Rate in various Hospitals .


## KEY INSIGHTS :

## 1 - Most type of cases admitted

### Elective Cases which is 18,655 i.e. 33.61% of the total cases followed by Urgent(18,576-33.47%) & Emergency((18,269-32.92%).

![img_04](https://github.com/user-attachments/assets/d9aa649d-8dab-4528-be42-6e7ac4ec836f)

## 2 - Age_Group with most Amount of Cases

###  Most Cases are form the 51-60 age group consist of 8,297
(Urgent-2,765, Emergency-2,657 & Elective-2,875).

![img_05](https://github.com/user-attachments/assets/a73bb60b-21a6-46b7-840f-95d1e2d83338)

## Most from Urgent are for obesity-514, Emergency(Athritis-478) & Urgent(Diabetes-502).

![img_5 5](https://github.com/user-attachments/assets/fd5d87b7-4749-4f79-99fe-e0d49654d1b6)

## 3 - Count of patients from Gender are

### Males consisting of 27,774 (50.04%) and Females 27,726(49.96%)

![img_03](https://github.com/user-attachments/assets/70c9506a-2d03-4065-92f8-2bd0bd6ed3a1)
 

### Males Majorly Suffering from Diabetes & Hypertension Where else Females from Arthritis

![img_03](https://github.com/user-attachments/assets/70c9506a-2d03-4065-92f8-2bd0bd6ed3a1)

## 4 - Most Cases as per Medical Condition
 
### Most Medical Cases comes from Arthritis(9308) & Diabetes(9304) 

![img_01](https://github.com/user-attachments/assets/cb2b5f09-ed09-4187-8d7f-7e81ea504639)

## 5 - Periodic Cases from 2020 to 2023

### Hypertension then Obesity being the top Cases form Year 2020 to 2021(FY-2021 QTR 4) to 2022 (FY-2022 QTR 1)
### Then a Sudden Increase in Diabetes from 2022 (FY-2022 QTR 2,3) till 2023(FY-2023 QTR 1)

## 6 - Avg Days For Discharge/Treatment for various Medical Conditions

### Asthma being the most with ~16 Days followed by Arthritis ~15 Days

## 7 - Insurance Companies and the Amount/Percent Amount Insured for medical Conditions

###Aetna being the most amount covering Provider with 93% of the Total Expenses followed by Cigna at 83%

## 8 - Medical Conditions and their expenses

### Obesity being the most Expensive Condition then Diabetes.

