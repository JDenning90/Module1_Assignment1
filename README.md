# Module1_Assignment1
## About
This assignment explores a series of hospital datasets and uses a series of SQL queries to extract the following information:
- List all doctors based at a particular hospital
- List all prescriptions for a specific patient, ordered by prescription date
- List all prescriptions prescribed by a specific doctor
- Add a new patient to the database and register them to a doctor
- Identify the doctor who has made the most prescriptions
- List all doctors at the hospital with the largest number of beds

A series of SQL queries were written and can be found in the [SQL_code.txt file](https://github.com/JDenning90/Module1_Assignment1/blob/main/SQL_code.txt). Each question has been listed with the relevant code beneath.
The project was planned using a mixture of [general planning notes and pseudocode](https://github.com/JDenning90/Module1_Assignment1/blob/main/Module%201%20Assignment%201%20Plan.docx) and an [ERD](https://github.com/JDenning90/Module1_Assignment1/blob/main/Health_Data_ERD.pdf).
  

## Files used

Below describes the files that were used, the original column names and the subsequent updated column names, along with the assigned data types. For more information about data types and how the tables relate to one another see the [health_data ERD](https://github.com/JDenning90/Module1_Assignment1/blob/main/Health_Data_ERD.pdf).
The SQL databse was exported using mysqldump and can be found in [back_up_health.sql](https://github.com/JDenning90/Module1_Assignment1/blob/main/back_up_health.sql)

### Doctors - [doctors.csv](https://github.com/JDenning90/Module1_Assignment1/blob/main/doctors.csv)

Dataset with information about doctors including the following columns:

| person_id | name | date_of_birth | address | role | hospital_id |
|-----------|------|---------------|---------|------|-------------|

Column names were updated and datatypes assigned as follows:

 | Column name    | Data type   |
 |---------------|--------------|
 | doctor_id     | INT unsigned | 
 | doctor_name   | VARCHAR(150) |
 | date_of_birth | DATE         |
 | address       | VARCHAR(150) |
 | role          | VARCHAR(50)  |
 | hospital_id   | INT unsigned |




### Hospitals - [hospitals.csv](https://github.com/JDenning90/Module1_Assignment1/blob/main/hospitals.csv)

Dataset with information about hosptials including the following columns:

| hospital_id | name | address | size | type | accreditation_status |
|-------------|------|---------|------|------|----------------------|


Column names were updated and datatypes assigned as follows:

 | Column name            | Data type    |
 |------------------------|--------------|
 | hospital_id            | INT unsigned |
 | hospital_name          | VARCAHR(150) |
 | address                | VARCHAR(150) |
 | size                   | INT          |
 | type                   | VARCHAR(100) |
 | accreditation_status   | VARCHAR      |




### Patients - [patients.csv](https://github.com/JDenning90/Module1_Assignment1/blob/main/patients.csv)

Dataset with information about patients including the following columns:

| person_id | name | date_of_birth | address | role | doctor_id   |
|-----------|------|---------------|---------|------|-------------|

Column names were updated and datatypes assigned as follows:


 | Column name   | Data type    |
 |---------------|--------------|
 | patient_id    | INT unsigned | 
 | patient_name  | VARCHAR(150) |
 | date_of_birth | DATE         |
 | address       | VARCHAR(150) |
 | role          | VARCHAR(50)  |
 | doctor_id     | INT unisigned|




### Prescriptions - [prescriptions.csv](https://github.com/JDenning90/Module1_Assignment1/blob/main/prescriptions.csv)

Dataset with information about prescriptions including the following columns:

| prescription_id| patient_id |doctor_id | medication | prescription_date |
|----------------|------------|----------|------------|-------------------|

Column names were updated and datatypes assigned as follows:

 | Column name      | Data type    |
 |------------------|--------------|
 | prescription_id  | INT unsigned |
 | patient_id       | INT unsigned |
 | doctor_id        | INT unsigned |
 | medication       | VARCHAR(150) |
 | prescription_date| DATE         |


## AI use statement
I have provided the [AI use statement](https://github.com/JDenning90/Module1_Assignment1/blob/main/AI_Statement.txt) as needed.

