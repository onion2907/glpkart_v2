# GLPKart V2 Documentation

## Table of Contents
1. [Introduction](#introduction)
2. [Architecture](#architecture)
3. [User Flows](#user-flows)
4. [Database Schema](#database-schema)
5. [Setup Guide](#setup-guide)
6. [API Documentation](#api-documentation)
7. [Testing and Validation](#testing-and-validation)
8. [FAQs](#faqs)

---

## Introduction
Welcome to the GLPKart V2 documentation. This platform is designed for seamless interactions between patients and healthcare providers through WhatsApp.

## Architecture
### Overview
- **Client-Server Model**: The application utilizes a client-server architecture.
- **Technology Stack**: The backend is powered by Node.js and Express, with a MongoDB database.
- **Integration**: The WhatsApp API facilitates communication between doctors and patients.

### Components
- **Frontend**: WhatsApp interface.
- **Backend**: RESTful API, Authentication, Database Management.
- **Database**: MongoDB schema for users, appointments, and prescriptions.

## User Flows
### Patient Flow
1. **Signup/Login**
2. **Appointment Booking**
3. **Consultation**
4. **Prescription Management**

### Doctor Flow
1. **Login**
2. **View Appointments**
3. **Consultation**
4. **Manage Prescriptions**

## Database Schema
### Patients
- **Collection Name**: `patients`
- **Fields**: `patient_id`, `name`, `contact`, `medical_history`, `prescriptions`

### Doctors
- **Collection Name**: `doctors`
- **Fields**: `doctor_id`, `name`, `specialization`, `availability`, `appointments`

### Appointments
- **Collection Name**: `appointments`
- **Fields**: `appointment_id`, `patient_id`, `doctor_id`, `date_time`, `status`

## Setup Guide
### Prerequisites
- Node.js installed
- MongoDB setup

### Installation Steps
1. Clone the repository: `git clone https://github.com/onion2907/glpkart_v2`
2. Navigate to the project directory: `cd glpkart_v2`
3. Install dependencies: `npm install`
4. Configure environment variables in `.env`
5. Start the application: `npm start`

## API Documentation
- **POST /api/login**: User login.
- **GET /api/appointments**: Fetch appointments.
- **POST /api/prescriptions**: Create new prescription.

## Testing and Validation
- Unit tests using Jest.
- Integration tests for API endpoints.

## FAQs
- **How to reset password?**
  - Password reset functionality is available through the login page.
- **How to contact support?**
  - Support can be reached via the official WhatsApp number provided on the website.