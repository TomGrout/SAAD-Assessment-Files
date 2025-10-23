Use Case ID: UC-008
Use Case Name: View Complaint Status
Primary Actor: Consumer
Goal: To allow a consumer to check the current status and history of their submitted complaint.

Preconditions:
- Consumer is authenticated and authorised.
- At least one complaint has been previously submitted.

Postconditions:
- Consumer can view up-to-date complaint details, status, and progress history.

Main Flow:
1. Consumer logs into the web or mobile application.
2. Consumer navigates to “My Complaints”.
3. System retrieves complaints associated with the user’s account.
4. Consumer selects a complaint to view its details.
5. System displays complaint status, assigned staff, and latest updates.

Alternative Flows:
A1. 
1. Consumer messages help agent through email or phone, with details of complaint.
2. Help agent retrieves complaints associated with the user’s account from system.
3. System displays complaint status, assigned staff, and latest updates.
4. Agent informs consumer of complaint status.

A2. No complaints found - System displays appropriate message.
A3. Backend unavailable - System shows cached data or maintenance notice.