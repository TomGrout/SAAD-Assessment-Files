Use Case ID: UC-006
Use Case Name: Onboard Tenant Organisation
Primary Actor: System Administrator
Goal: To register a new organisation (tenant) for use within the multi-tenant CMS.

Preconditions:
- Administrator is authenticated with admin privileges.
- System capacity allows for new tenant creation.

Postconditions:
- New tenant record created with isolated data store/ schema.
- Initial users and permissions configured.

Main Flow:
1. Administrator accesses the tenant management interface.
2. Administrator enters organisation details and configuration.
3. System validates and provisions tenant schema and storage.
4. System confirms successful onboarding.

Alternative Flows:
A1. Invalid configuration - System rejects request and prompts correction.
A2. Provisioning error - System logs failure and notifies administrator.
A3. Validation error - System rejects invalid or duplicate tenant.