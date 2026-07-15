# Database Design

## Core Tables

### 1. Users
Stores registered users.

Fields:
- user_id
- full_name
- email
- phone
- password
- role
- is_anonymous
- created_at

---

### 2. Community Reports
Stores crime reports submitted by citizens.

Fields:
- report_id
- user_id
- crime_type_id
- state_id
- city_id
- title
- description
- location
- latitude
- longitude
- status
- submitted_at

---

### 3. Crime Cases
Stores verified and famous crime cases.

Fields:
- case_id
- title
- description
- crime_type_id
- state_id
- city_id
- case_status
- verdict
- court_name
- year
- ai_summary
- source
- created_at

---

### 4. Crime Types

Fields:
- crime_type_id
- crime_name

Examples:
- Murder
- Cyber Crime
- Fraud
- Kidnapping
- Domestic Violence
- Human Trafficking

---

### 5. States

Fields:
- state_id
- state_name

---

### 6. Cities

Fields:
- city_id
- state_id
- city_name

---

### 7. Evidence

Fields:
- evidence_id
- report_id
- file_type
- file_path
- uploaded_at

---

### 8. Safety Articles

Fields:
- article_id
- title
- category
- content
- created_at

---

### 9. Admins

Fields:
- admin_id
- name
- email
- password

---

### 10. AI Logs

Fields:
- log_id
- case_id
- generated_summary
- generated_at
