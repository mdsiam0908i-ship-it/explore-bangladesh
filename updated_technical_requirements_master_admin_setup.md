# Technical Requirements & System Architecture: Bangladesh Travel Guide App

## 1. System Architecture
- **Frontend:** Flutter or React Native (for cross-platform iOS/Android support).
- **Backend:** Node.js with Express.
- **Database:** PostgreSQL (Relational) or Firebase Firestore (NoSQL) for real-time SOS features.
- **Authentication:** JWT-based secure authentication with multi-factor support.
- **Infrastructure:** AWS or Google Cloud Platform.

## 2. Database Schema (Core Tables)

### Users Table
| Field | Type | Description |
|---|---|---|
| id | UUID | Primary Key |
| full_name | String | User's full legal name |
| username | String | Unique username |
| password_hash | String | Bcrypt hashed password |
| email | String | Unique verified email |
| dob | Date | Date of Birth |
| user_type | Enum | 'BD_Citizen', 'Foreigner', or 'Admin' |
| phone_primary | String | Mandatory phone number |
| phone_secondary | String | Optional (for foreigners) |
| home_country | String | Country of origin |
| identity_type | String | 'Passport', 'NID', 'Travel_ID' |
| identity_id | String | Identity document number |
| created_at | Timestamp | Account creation date |
| role | Enum | 'USER', 'MERCHANT', 'ADMIN', 'SUPER_ADMIN' |

### Emergency_Alerts Table
... (rest of table)

## 3. UI/UX Workflow
... (rest of workflow)

## 4. Initial System Configuration (Seed Data)
- **Master Admin Account:**
  - **Username:** `exbsiam`
  - **Password:** `siqm09L0@#` (Example for prototype; stored hashed in production)
  - **Role:** `SUPER_ADMIN`
  - **Permissions:** Full access to Global Settings, Payment Logic, User Management, and SOS Controls.
