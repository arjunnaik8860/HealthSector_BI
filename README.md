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

![Image](https://github.com/user-attachments/assets/981b23ce-deba-435e-9ef2-a02cc8203f9c)

## 2 - Age_Group with most Amount of Cases

###  Most Cases are form the 51-60 age group consist of 8,297
(Urgent-2,765, Emergency-2,657 & Elective-2,875).
![Image](https://github.com/user-attachments/assets/9591e976-7120-46ba-83b2-ccc28979cc7b)

## Most from Urgent are for obesity-514, Emergency(Athritis-478) & Urgent(Diabetes-502).

![Image](https://github.com/user-attachments/assets/1c2a9fd7-6f2f-479b-becb-5527c061b98f)
![Image](https://github.com/user-attachments/assets/e4d807ea-6a83-42cb-bd29-0b10f7d5d4ef)
![Image](https://github.com/user-attachments/assets/448aa605-4cbc-479a-bebc-52873d85c862)

## 3 - Count of patients from Gender are

### Males consisting of 27,774 (50.04%) and Females 27,726(49.96%)

![Image](https://github.com/user-attachments/assets/4e44c5fc-d025-485f-b0b0-193b6b481e99)
![Image](https://github.com/user-attachments/assets/5ea5751f-1718-41ac-a9b0-cfed3c18b8e9) 

### Males Majorly Suffering from Diabetes & Hypertension Where else Females from Arthritis

## 4 - Most Cases as per Medical Condition
 
### Most Medical Cases comes from Arthritis(9308) & Diabetes(9304) 

![Image](https://github.com/user-attachments/assets/f894cc4b-14b5-4471-b093-38e0b8ae1747)

## 5 - Periodic Cases from 2020 to 2023

### Hypertension then Obesity being the top Cases form Year 2020 to 2021(FY-2021 QTR 4) to 2022 (FY-2022 QTR 1)
![Image](https://github.com/user-attachments/assets/ea0a6749-cf44-49d0-a9a5-93ff447b69d0)
### Then a Sudden Increase in Diabetes from 2022 (FY-2022 QTR 2,3) till 2023(FY-2023 QTR 1)

## 6 - Avg Days For Discharge/Treatment for various Medical Conditions

### Asthma being the most with ~16 Days followed by Arthritis ~15 Days

![Image](https://github.com/user-attachments/assets/7530e196-b93a-4e35-9737-69adc32c2d55)

## 7 - Insurance Companies and the Amount/Percent Amount Insured for medical Conditions

###Aetna being the most amount covering Provider with 93% of the Total Expenses followed by Cigna at 83%

![Image](https://github.com/user-attachments/assets/d71dcde2-f1d6-4f9d-af82-a4289b7dff9c)

## 8 - Medical Conditions and their expenses

### Obesity being the most Expensive Condition then Diabetes.

![Image](https://github.com/user-attachments/assets/d900404c-792d-4ddb-a769-df5d0a535550)

