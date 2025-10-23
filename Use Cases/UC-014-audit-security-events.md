Use Case ID: UC-014
Use Case Name: Audit Security Events
Primary Actor: System Administrator
Goal: To review security-related events and ensure compliance with organisational policies.

Preconditions:
- Audit logging enabled and present in Azure Monitor.
- System generates structured audit logs for authentication and authorisation events.
- Administrator has audit viewing permissions.

Postconditions:
- Security events are reviewed and exported for compliance reporting.

Main Flow:
1. Administrator accesses audit and monitoring console.
2. Administrator filters events by user, tenant, or date range.
3. System retrieves logs from Azure Monitor.
4. Administrator reviews key events such as login attempts, access denials, and configuration changes.
5. Administrator reviews and exports report for compliance records.

Alternative Flows:
A1. Log retrieval failure - System displays error and logs issue.
A2. No matching records - System displays “no results found”.
A3. Suspicious pattern detected - System alerts administrator.