# MedtechAnalysis
MedTech Database Project Outline
Tables:

Patients

patient_id (PK)
patient_name
date_of_birth
gender
contact_number
address
email

Doctors

doctor_id (PK)
doctor_name
specialization
contact_number
email

Appointments

appointment_id (PK)
patient_id (FK to Patients)
doctor_id (FK to Doctors)
appointment_date
appointment_time
status (scheduled, completed, canceled, etc.)
reason_for_visit

MedicalRecords

record_id (PK)
patient_id (FK to Patients)
doctor_id (FK to Doctors)
appointment_id (FK to Appointments)
record_date
symptoms
diagnosis
treatment
prescription
