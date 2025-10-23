Use Case ID: UC-013
Use Case Name: Receive Complaint Notifications
Primary Actor: Consumer
Goal: To receive timely updates on complaint lifecycle (creation, assignment, progress, and resolution).

Preconditions:
- Consumer has a valid communication channel (email, SMS, or app notification).
- Notifications are enabled in tenant configuration.
- Complaint event occurs (creation, assignment, progress resolution).

Postconditions:
- Consumer receives relevant updates triggered by complaint status changes.

Main Flow:
1. Complaint event occurs in the system.
2. Event is published to the message queue.
3. Notification service sees the event and formats the message.
4. System sends notification through channel (Twilio).
3. Channel sends message via SMS, email, or push notification.
5. Consumer receives notification.

Alternative Flows:
A1. Assisted Communication - Help Desk Agent manually contacts consumer via phone or email.
A2. Notification channel unavailable - System retries or switches to fallback channel, logs failure.
A3. Consumer opted out - System skips notification.
