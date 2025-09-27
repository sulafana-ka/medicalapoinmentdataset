# medicalapoinmentdataset
clean and prepared dataset

🎯 Overview

This repository houses the raw and cleaned versions of the medicalappointment dataset ('raw data medicalappoinment.csv'). The cleaning and formatting process was performed manually using Micrisoft Excel to prepare the data for subsequent analysis and development focused on predicting patient no-shows.

📊 Data Source

-Raw File: 'raw data medicalappoinment.csv'

-Cleaned File: 'medicalappoinment data.xlsx'

-Description: Contains over 110,000 records of medical appointments in Brazil, including patient demographics, scheduling information, and the final attendance status.

✨ Data Cleaning and Formatting Steps

The following manual steps were executed in Excel to ensure data quality and consistency:

1. Data Type Conversion & Formatting
   
*Date Formatting:

 -The ScheduledDay and AppointmentDay columns were converted from text to Date/Time format.

 -The time component was removed from AppointmentDay since all records had 00:00:00Z, simplifying it to only the date (e.g., YYYY-MM-DD).

*ID Formatting:

 -The PatientId column was formatted to remove scientific notation (e.g., 2.98725E+13), ensuring the full 15-digit ID is displayed as a number.

*Data Encoding:

 -The gender column ('F/M') was converted to a full form as ('Male and Female')for easier analysis. 

2. Data Validation and Error Handling
   
 -Age Check: Used a filter to locate and investigate rows where the Age was negative or zero. Invalid age records were handled by removal (or noted).

 -Duplicate Check: Used Excel's Conditional Formatting to highlight and remove any fully duplicated rows.

🚀 Usage and Next Steps

The cleaned file medicalappointmentdata.xlsx , is now ready for use in any data analysis or modeling environment (e.g., Python, R, Tableau, etc.).

 1.Download the 'medicalappointment data.xlsx' file.

 2.Import it into your preferred analysis tool.

 3.Begin Exploratory Data Analysis (EDA).


