Use Case ID: UC-004
Use Case Name: Confirm Resolution
Primary Actor: Consumer
Goal: To confirm whether a reported issue has been successfully resolved, either online or via email/message.

Preconditions:
- Complaint status is “Resolved – Pending Confirmation”.
- Consumer is notified of resolution.

Postconditions:
- Complaint status updated to “Closed” upon confirmation.
- Feedback and satisfaction rating recorded.

Main Flow:
1. Consumer opens resolution notification.
2. Consumer logs in and reviews complaint details.
2. Consumer reviews issue and provides confirmation and (optionally) feedback.
3. System records confirmation and updates complaint status.
4. Consumer receives closure acknowledgement.

Alternative Flows:
A1. Consumer rejects resolution - System reopens complaint for reassignment.
A2. No response after defined period - System auto-closes complaint.
A3. Assisted Confirmation:
   1. Consumer calls or emails help desk.
   2. Agent retrieves complaint and records consumer’s verbal confirmation.
   3. System closes complaint and notifies consumer.