Use Case ID: UC-002
Use Case Name: Assign Complaint
Primary Actor: Help Desk Agent
Goal: To allocate a complaint to a suitable support person for resolution.

Preconditions:
- Complaint exists with status “Open”.
- Help Desk Agent is authenticated and authorised.

Postconditions:
- Complaint status is updated to “Assigned”.
- Assigned support person receives notification.

Main Flow:
1. Help Desk Agent views list of open complaints.
2. Agent reviews complaint details and selects appropriate support person.
3. System updates assignment details and status.
4. Notification is sent to the assigned support person.

Alternative Flows:
A1. No available support person – System flags for manager review.
A2. Agent lacks permission – System denies access and logs event.
