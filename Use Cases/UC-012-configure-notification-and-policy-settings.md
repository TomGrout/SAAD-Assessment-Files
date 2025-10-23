Use Case ID: UC-012
Use Case Name: Configure Notification and Policy Settings
Primary Actor: System Administrator
Goal: To manage global or tenant-level configurations for notifications, SLA thresholds, and policies.

Preconditions:
- Administrator has super-admin or tenant-admin privileges.
- Tenant or system instance exists, configuration is available.

Postconditions:
- Updated configuration stored and applied across relevant modules.

Main Flow:
1. Administrator accesses system configuration.
2. Administrator selects notification, SLA or policy settings.
3. Administrator modifies configuration parameters (email templates, thresholds, retry limits, user preferences).
4. System validates configuration and applies updates.
5. System logs change and notifies affected services & stakeholders.

Alternative Flows:
A1. Invalid configuration - System rejects changes and provides validation feedback.
A2. Update failure - System rolls back to last known valid configuration.
