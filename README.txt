TaskFlow V2 — RBAC, User Management, History & Attachments

This build includes:
- DB-driven login and role routing.
- Logout and self-service password change for every authenticated user.
- TL-only User Management with creation of AGENT, TL and RTM accounts.
- TL user activation/deactivation and deletion through the protected Supabase Edge Function.
- Ticket fields: Title, Assign to, Priority, Deadline, Description, Attachments.
- Image attachments, external links, and pasted clipboard images (Ctrl+V / Cmd+V).
- Ticket history timeline with creator name + role, events, assignments and comments.
- Attachment history with uploader name + role.
- Private Supabase Storage bucket: ticket-attachments (10 MB/file).
