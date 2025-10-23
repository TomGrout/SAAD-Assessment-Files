Use Case ID: UC-002
Use Case Name: Assign Complaint
Primary Actor: Help Desk Agent
Goal: To allocate a complaint to the most suitable support person for resolution.

Preconditions:
- Complaint exists with status “Open”.
- Help Desk Agent is authenticated and authorised.

Postconditions:
- Complaint status is updated to “Assigned”.
- Assigned support person and consumer receive notification.

Main Flow:
1. Help Desk Agent views list of open complaints.
2. Agent reviews details and selects “Assign”.
3. System suggests available support persons based on workload distribution.
4. Agent confirms assignment.
5. System updates record and sends notifications.

Alternative Flows:
A1. Manual Assignment via Call - Agent receives phone request and performs assignment while on call.
A2. No available support person - System flags for manager review.
A3. Agent lacks permission - System denies access and logs event.
