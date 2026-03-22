# CivicFlow - MongoDB Schema Design

## Collections

### 1.Procedures
- procedure_id, category, states[], created_at

### 2.States (inside procedure)
- state_id, name, required_documents[], timeline, authority, fees, next_states[]

### 3.Complaints
- complaint_id, user_id, category, current_state, status, created_at, updated_at

### 4.User_sessions
- session_id, user_id, procedure_id, current_step, started_at

### 5.Document_checklists
- checklist_id, complaint_id, documents[{name, required, uploaded}]
