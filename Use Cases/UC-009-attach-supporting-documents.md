Use Case ID: UC-009
Use Case Name: Attach Supporting Documents
Primary Actor: Consumer
Goal: To allow consumers to upload files or images that support their complaint.

Preconditions:
- Consumer is authenticated.
- Consumer is logging a new complaint, or has an existing one with "Open" or "Assigned" status.

Postconditions:
- Files are securely stored in the system and linked to the relevant complaint record.

Main Flow:
1. Consumer opens complaint details.
2. Consumer selects “Attach Files".
3. System prompts for file upload.
4. Consumer uploads one or more files.
5. System validates file type and size.
6. System stores files in secure blob storage and updates complaint record.
7. Consumer receives confirmation of successful upload.

Alternative Flows:
A1. Invalid file type or size - System displays error message.
A2. Network interruption - System retries or prompts user to re-upload.
