## Overview of the Project
The purpose of this assignment is to be able to read patients.csv with python/SQLite so that we can run and analyze queries through DBBrowser
## Steps to recreate the database
1. Recreate repository with appropriate python script files and make sure that Python, Pandas, SQLAlchemy are installed and install dependencies via requirements.txt.
2. Place patients.csv in data folder
3. Run src/create_db.py to create database
4. Run src/import_csv.py to load to CSV
5. Open clinic_simple.db in DB Browser for SQLite and run sql/analysis.sql queries

## Query results
### A
This counts the total number of patients in the CSV data (500).
![resultA](images/result_A.png)

### B
This totals the number of patients in each icd-10 category and lists them in descending order
![resultB](images/result_B.png)

### C
This lists the patients where their last CPT code starts with 992 and visited after the date 1/1/25. It lists in descending order with most recently visited patient showing at the top.
![resultC](images/Results_C.png)

### D
This shows the five oldest patients at the time of visit in the list. All five patients are the same age but it is designed to list them in descending age order, with oldest being at the top.
![resultD](images/Results_D.png)

### E
This tries to see if any CPT or ICD-10 codes are missing in the list. However, the results show that there are no blanks.
![resultE](images/Results_E.png)
