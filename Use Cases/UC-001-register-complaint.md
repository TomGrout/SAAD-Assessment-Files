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
1. Consumer opens web or mobile interface and selects “New Complaint”.
2. System prompts for relevant details (category, description, contact information, relevant files).
3. Consumer submits complaint.
4. System validates data and stores the complaint record in tenant-specific schema.
5. System sends confirmation notification to consumer by email or SMS.

Alternative Flows:
A1. Assisted Contact:
   1. Consumer contacts help desk via phone or email.
   2. Help Desk Agent records complaint details on behalf of consumer.
   3. System stores complaint and provides reference number.
   4. Agent communicates reference back to consumer.

A2. Invalid or incomplete data - System requests corrections before submission.
A3. Network or service interruption - System queues submission and notifies user of delay.
A4. Accessibility mode enabled - Interface adjusts layout per WCAG 2.2 AA guidelines.
