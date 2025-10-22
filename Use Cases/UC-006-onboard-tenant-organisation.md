Use Case ID: UC-006
Use Case Name: Onboard Tenant Organisation
Primary Actor: System Administrator
Goal: To register a new organisation (tenant) for use within the multi-tenant CMS.

Preconditions:
- Administrator is authenticated with super-admin privileges.
- System capacity and configuration allow for new tenant creation.

Postconditions:
- New tenant record created with isolated data store.
- Initial users and permissions configured.

Main Flow:
1. Administrator accesses the tenant management interface.
2. Administrator enters organisation details and configuration parameters.
3. System validates and provisions tenant environment.
4. System confirms successful onboarding and notifies relevant stakeholders.

Alternative Flows:
A1. Invalid configuration – System rejects request and prompts correction.
A2. Provisioning error – System logs failure and notifies administrator.
