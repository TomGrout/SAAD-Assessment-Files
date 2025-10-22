Use Case ID: UC-001
Use Case Name: Register Complaint
Primary Actor: Consumer
Goal: To allow a consumer to log a complaint through the web or mobile application.

Preconditions:
- Consumer has valid access to the system.
- The system is available and operational.

Postconditions:
- Complaint is recorded with unique identifier and initial status “Open”.
- Consumer receives confirmation via email or SMS.

Main Flow:
1. Consumer navigates to the complaint submission form.
2. System prompts for relevant details (category, description, contact information).
3. Consumer submits complaint.
4. System validates data and stores the complaint record.
5. System sends confirmation notification to consumer.

Alternative Flows:
A1. Invalid Data – System displays validation error and requests correction.
A2. System Error – System logs issue and displays error message to user.
