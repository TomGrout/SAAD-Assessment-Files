Use Case ID: UC-003
Use Case Name: Resolve Complaint
Primary Actor: Support Person
Goal: To resolve an assigned complaint and update its resolution details.

Preconditions:
- Complaint is assigned to the support person.
- Support person has required access rights.

Postconditions:
- Complaint record updated with resolution notes and status “Resolved – Pending Confirmation”.
- Consumer is notified of the resolution & resolution summary.

Main Flow:
1. Support person reviews assigned complaints.
2. Support person investigates and performs resolution steps.
3. Support person records resolution remarks.
4. System updates status and notifies consumer of resolution.
5. Resolution analytics are logged.

Alternative Flows:
A1. Resolution cannot be completed - Support person escalates to Help Desk Manager (see UC-010).
A2. System unavailable - Changes queued for later synchronisation.
A3. Assisted Resolution - Support person collaborates with agent through internal chat or call.