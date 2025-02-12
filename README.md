# PySQLite_EHR_System
This project is a simple Electronic Health Record (EHR) System built using SQLite and Python. It allows healthcare providers to register new patients, record consultations with health complaints, document medical services provided during consultations, and retrieve a patient's consultation history. The system is designed for easy use and interaction with a terminal-based interface.

## Features
- Register New Patient: Add patient details, including personal information, contact details, and gender.
- Record Consultation: Log consultations with health complaints, linking them to a patient.
- Record Medical Services: Document services provided during consultations, including prescribed medications and service descriptions.
- View Consultation History: Retrieve and display the consultation history of any patient with details of services and medications.

## Database Structure

The system uses an SQLite database with the following tables:

1. Company_Info: Stores information about the healthcare company (optional, for future expansion).
2. Patient: Contains patient details such as name, date of birth, gender, contact information, etc.
3. Consultation_Record: Logs consultation data, including health complaints and the consultation date.
4. Medical_Service: Stores details about services provided during consultations, such as prescribed medications.
5. Patient_Consultation_History: Links patient IDs with consultation IDs, storing the timestamp of each consultation.

## Requirements

- Python 3.x
- SQLite (integrated with Python's `sqlite3` module)

## Installation

1. Clone this repository to your local machine:
   ```
   git clone https://github.com/your-username/ehr-system.git
   ```

2. Navigate to the project directory:
   ```
   cd ehr-system
   ```

3. Ensure that Python 3.x is installed on your machine. If not, [download and install Python 3](https://www.python.org/downloads/).

4. Run the system:
   ```
   python ehr_system.py
   ```

   The system will create the SQLite database (`ehr_system.db`) and allow you to interact with it through the command-line interface.

## How to Use

Upon running the program, you'll be presented with a simple menu with the following options:

1. Register New Patient: Input patient details to register them in the system.
2. Record Consultation and Health Complaints: Enter a consultation record for a specific patient, including complaints and the consultation date.
3. Record Medical Services Provided: Log the medical services provided (e.g., prescribed medications) for a given consultation.
4. **View Patient's Consultation History**: Retrieve a patient's consultation history along with the details of services provided.
5. **Exit**: Exit the application.

### Example Interaction:

1. Register a new patient:
   ```
   Enter patient's first name: John
   Enter patient's last name: Doe
   Enter patient's date of birth (YYYY-MM-DD): 1985-05-15
   Enter patient's gender (Male | Female): Male
   Enter patient's address: 123 Main St, City
   Enter patient's contact number: 123-456-7890
   ```

2. Record a consultation:
   ```
   Enter the health complaints discussed with the physician: Persistent headache
   ```

3. Record a medical service:
   ```
   Enter the service description provided by the physician: General checkup
   Enter the prescribed medication (if any): Acetaminophen
   ```

4. View patient history:
   ```
   Consultation ID: 1
   Complaints: Persistent headache
   Consultation Date: 2025-02-12 14:00:00
   Medical Service: General checkup
   Prescribed Medication: Acetaminophen
   ```

## File Structure

- `ehr_system.py`: Main Python script that contains the logic for the EHR system.
- `ehr_system.db`: SQLite database where patient, consultation, and medical service records are stored.
  

---


