# Biometric-Fingerprint-Service-Platform
End-to-end fingerprint verification system using Angular, Spring Boot, MySQL, and SourceAFIS
## Description
This project is an **end-to-end biometric fingerprint verification system** developed during my internship.  
It allows real-time fingerprint capture, registration, and verification using a modular frontend-backend setup.

- **Frontend:** Angular  
- **Backend:** Java Spring Boot  
- **Database:** MySQL  
- **Fingerprint Algorithm:** SourceAFIS  

---

## Features
- **Capture Fingerprints:** Supports left and right hand finger/thumb capture.  
- **Display Scanned Images:** Shows BMP Base64 fingerprint images in real-time.  
- **User Management:** Register, edit, and update user info along with fingerprints.  
- **Fingerprint Verification:** Matches captured fingerprint against stored templates using SourceAFIS.  
- **Secure Storage:** Fingerprints saved as Base64 and SourceAFIS templates in database.  
- **Instant Feedback:** Displays match results (`Match Found` / `No match found`) immediately.  

---

## Installation

### Step 1 – Install Drivers & WebAPI
1. Create a folder named **Drivers** containing:  
   - **SecuGen WebAPI:** [Download](https://webapi.secugen.com/Demo1)  
   - **SecuGen Drivers:**  
     - SecuGenLegacyDriverInstaller_22  
     - SecuGenWBFDriverInstaller_25  
     [Driver Download](https://secugen.com/drivers/)  
2. Verify installation using: [Demo WebAPI](https://webapi.secugen.com/Demo1)  

### Step 2 – Backend Setup
1. Navigate to the backend folder:
   ```bash
   cd springboot-backend
   Build and run Spring Boot application:
   mvn clean install
mvn spring-boot:run
****Step 3 – Frontend Setup****
Navigate to the frontend folder:
cd angular-frontend
Install dependencies:
npm install
Run the Angular application:
ng serve
Open in browser: http://localhost:4200

****Usage****

-Open the User List component to view all users.

-Click Edit to modify user info → opens Register Component.

-Capture fingerprints using Verify Fingerprint button.

-Fill in or edit Name, CNIC, Age, etc.

-Press Register / Update → saves user info and fingerprints to database.

-Use Verify Fingerprint to match captured fingerprint against stored templates.

