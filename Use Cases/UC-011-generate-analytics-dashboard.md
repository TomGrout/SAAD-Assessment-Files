Use Case ID: UC-011
Use Case Name: Generate Analytics Dashboard
Primary Actor: Help Desk Manager
Goal: To visualise complaint data and performance metrics.

Preconditions:
- Manager is authenticated and authorised.
- Reporting store contains relevant data.

Postconditions:
- Dashboard generated and displayed with interactive charts.

Main Flow:
1. Manager opens the analytics dashboard interface.
2. Manager selects reporting parameters (date range, department, tenant).
3. System queries the reporting store.
4. System visualises metrics such as average resolution time, open complaints, and satisfaction scores.
5. (Optional) Manager exports or downloads dashboard insights.

Alternative Flows:
A1. Data unavailable - System displays “no data” message.
A2. Report generation timeout - System retries and logs the event.
A3. Report timeout - System retries with smaller dataset.
A4. Accessibility tools enabled - Dashboard adjusts for screen readers.