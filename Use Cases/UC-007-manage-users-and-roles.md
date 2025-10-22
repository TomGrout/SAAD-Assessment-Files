Use Case ID: UC-007
Use Case Name: Manage Users and Roles
Primary Actor: System Administrator
Goal: To manage users, roles, and permissions for all tenants.

Preconditions:
- Tenant exists and has active users.
- Administrator has the required privileges.

Postconditions:
- User accounts and access roles are updated accordingly.
- Audit log records all administrative actions.

Main Flow:
1. Administrator views list of users under a tenant.
2. Administrator creates, edits, or removes users.
3. Administrator assigns or modifies roles.
4. System validates updates and persists changes.
5. System records changes in audit log.

Alternative Flows:
A1. Invalid input – System displays error message and requests correction.
A2. Operation not permitted – System denies action and logs event.
