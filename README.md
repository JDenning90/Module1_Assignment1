# Module1_Assignment1
## About
This assignment explores a series of hospital datasets and extracts the follwoing information:
- List all doctors based at a particular hospital
- list all prescriptions for a specific patient, ordered by prescription date
- list all prescriptions prescribed by a specific doctor
- Add a new patient to the database and register them to a doctor
- Identify the docotr who has made the most prescriptions
- list all doctors at the hospital with the largest number of beds
  

## Files used
### Doctors - doctors.csv

| person_id | name | date_of_birth | address | role | hospital_id |
|-----------|------|---------------|---------|------|-------------|

### Hospitals - hospitals.csv
| hospital_id | name | address | size | type | accreditation_status |
|-------------|------|---------|------|------|----------------------|


### Patients - patients.csv
| person_id | name | date_of_birth | address | role | doctor_id   |
|-----------|------|---------------|---------|------|-------------|

### Prescriptions - prescriptions.csv
| prescription_id| patient_id |doctor_id | medication | prescription_date |
|----------------|------------|----------|------------|-------------------|

## Database
Describe and include what the tables are

Include info on how to use the files and what the queries are

Describe purpose of each SQL query

