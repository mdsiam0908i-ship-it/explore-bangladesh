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
| user_type | Enum | 'BD_Citizen' or 'Foreigner' |
| phone_primary | String | Mandatory phone number |
| phone_secondary | String | Optional (for foreigners) |
| home_country | String | Country of origin |
| identity_type | String | 'Passport', 'NID', 'Travel_ID' |
| identity_id | String | Identity document number |
| created_at | Timestamp | Account creation date |

### Emergency_Alerts Table
| Field | Type | Description |
|---|---|---|
| id | UUID | Primary Key |
| user_id | UUID | Foreign Key to Users |
| category | Enum | Danger category (e.g., Medical, Crime, Accident) |
| description | Text | User's typed details |
| gps_lat | Decimal | Current latitude |
| gps_long | Decimal | Current longitude |
| status | Enum | 'Pending', 'Active', 'Resolved' |
| responder_id | UUID | Admin/Merchant ID handling the case |

### Routes Table
| Field | Type | Description |
|---|---|---|
| id | UUID | Primary Key |
| origin | String | Location A |
| destination | String | Location B |
| transport_modes | Array | Available transport types |
| estimated_fare | Decimal | Current fair/rent cost |
| pros | Text | Positive aspects |
| cons | Text | Risks/Bad aspects |

## 3. UI/UX Workflow

### Phase 1: Onboarding
1. **Splash Screen:** App branding.
2. **Login Screen:** Username/Password + Admin Login toggle.
3. **Sign-Up Type:** Choose "BD Citizen" or "Foreigner".
4. **Registration Form:** Context-aware fields based on user type.
5. **Identity Verification:** Document upload/entry.

### Phase 2: Home & Core Features
1. **Home Screen:** Seasonal Banner (Top) + Quick Actions (SOS, Translator, Planner).
2. **Route Planner:** Multi-step journey input and detail output.
3. **Travel Tools:** Regional Translator (Speech output) & Currency Converter.
4. **Account Center:** Profile management and registration updates.

### Phase 3: Emergency (SOS)
1. **SOS Trigger:** Prominent Help button.
2. **Incident Report:** Category selection + Live tracking toggle.
3. **Emergency Call:** Direct 999 dialer interface.
