# Airtable Schema Documentation

## Tables

### 1. Patients  
- **Fields**:  
  - `Patient ID`: Unique identifier for each patient.  
  - `Name`: Full name of the patient.  
  - `Date of Birth`: Patient's birth date.  
  - `Contact Information`: Phone number and email address.  
  - `Address`: Residential address.  
  
### 2. Consultations  
- **Fields**:  
  - `Consultation ID`: Unique identifier for each consultation.  
  - `Patient ID`: Reference to the patient.  
  - `Doctor ID`: Reference to the doctor conducting the consultation.  
  - `Consultation Date`: Date and time of the consultation.  
  - `Notes`: Additional notes or findings from the consultation.  
  
### 3. Prescriptions  
- **Fields**:  
  - `Prescription ID`: Unique identifier for each prescription.  
  - `Consultation ID`: Reference to the related consultation.  
  - `Doctor ID`: Reference to the prescribing doctor.  
  - `Medicines`: List of prescribed medicines.  
  - `Dosage Instructions`: Instructions on how the medicines should be taken.  
  
### 4. Orders  
- **Fields**:  
  - `Order ID`: Unique identifier for each order.  
  - `Patient ID`: Reference to the patient placing the order.  
  - `Medicine ID`: Reference to the ordered medicine.  
  - `Quantity`: Number of units ordered.  
  - `Order Date`: Date when the order was placed.  
  
### 5. Doctors  
- **Fields**:  
  - `Doctor ID`: Unique identifier for each doctor.  
  - `Name`: Full name of the doctor.  
  - `Specialization`: Medical specialty of the doctor.  
  - `Contact Information`: Phone number and email address.  
  
### 6. Pharmacy Partners  
- **Fields**:  
  - `Pharmacy ID`: Unique identifier for each pharmacy partner.  
  - `Name`: Name of the pharmacy.  
  - `Contact Information`: Phone number and email address.  
  
### 7. Medicines  
- **Fields**:  
  - `Medicine ID`: Unique identifier for each medicine.  
  - `Name`: Name of the medicine.  
  - `Description`: Description of the medicine.  
  - `Price`: Cost of the medicine.  
  
### 8. Payments  
- **Fields**:  
  - `Payment ID`: Unique identifier for each payment.  
  - `Order ID`: Reference to the related order.  
  - `Amount`: Total payment amount.  
  - `Payment Date`: Date and time of the payment.  
  - `Payment Method`: Method of payment (e.g., Credit Card, PayPal).  

---

Documentation last updated on **2026-04-06 06:25:13 UTC**.