TaskFlow — Client Role + Stuck Resolution Update

Changes in this build:
- Renamed the former RTM role to CLIENT in the database enum and UI.
- TL user management now creates/edits CLIENT accounts instead of RTM accounts.
- Updated the protected manage-taskflow-users Edge Function to accept CLIENT.
- Added "Resolved Without Return" for TL/CLIENT when a ticket is STUCK.
- Resolved Without Return moves the ticket to COMPLETED, records a dedicated audit event, keeps the stuck history, supports resolution attachments, and notifies the creator/assignee.
- Existing "Resolve & Return" behavior is preserved.
- Reassign labels no longer reference the old role name.
