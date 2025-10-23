Use Case ID: UC-010
Use Case Name: Escalate Complaint
Primary Actor: Help Desk Agent
Goal: To escalate unresolved or critical complaints to higher-level support or management.

Preconditions:
- Complaint exists with status “Assigned” or “In Progress”.

Postconditions:
- Complaint status updated to “Escalated”.
- Notification sent to assigned manager or escalation team.

Main Flow:
1. Help Desk Agent reviews complaint resolution history.
2. Agent identifies need for escalation based on SLA breach or customer dissatisfaction.
3. Agent selects “Escalate” option and provides reason.
4. System updates complaint status and assigns it to escalation queue.
5. System notifies relevant stakeholders (higher-level support or management) via email or SMS.

Alternative Flows:
A1. Automatic Escalation - System triggers escalation when SLA breached for too long.
A2. Escalation via call - Agent notifies manager directly by phone; system updated manually afterward.
A3. Escalation rejected - Manager reviews and returns complaint.
