Use Case ID: UC-004
Use Case Name: Confirm Resolution
Primary Actor: Consumer
Goal: To confirm whether a reported issue has been successfully resolved.

Preconditions:
- Complaint status is “Resolved – Pending Confirmation”.
- Consumer is notified of resolution.

Postconditions:
- Complaint status updated to “Closed” upon confirmation.
- Feedback and satisfaction rating recorded.

Main Flow:
1. Consumer receives resolution notification.
2. Consumer reviews issue and provides confirmation or feedback.
3. System records confirmation and updates complaint status.
4. Consumer receives closure acknowledgement.

Alternative Flows:
A1. Consumer rejects resolution – System reopens complaint for reassignment.
A2. No response after defined period – System auto-closes complaint.
