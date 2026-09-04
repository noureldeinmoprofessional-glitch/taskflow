TaskFlow V6 — notification + stuck workflow prototype

New in V6:
- Full Ticket timestamps: created, assigned, accepted, started, stuck, resolved, reassigned, completed.
- TL/RTM stuck actions: Resolve or Reassign.
- Reassign records old/new agent, time and reason.
- Resolve notifies the original agent.
- New assignment notifies the new agent.
- In-app notification bell with unread badge.
- Chrome Browser Notification permission flow using the Web Notifications API.
- Toast + in-app notification + browser notification for task events.
- Deadline warning under 15 minutes.
- Demo localStorage persistence.

Demo:
TL / 1234
RTM / 1234
AGENT / 1234

Important:
This is still a front-end prototype. For production, replace localStorage with Supabase/Postgres + Supabase Auth + RLS + server-side user provisioning + Supabase Realtime. For notifications while the site is closed, add a service worker + Push API (Web Push) and a backend sender. Browser notifications require user permission and HTTPS in production.
