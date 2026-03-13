# Power Automate Flows

This document defines the automation workflows used by the Productivity Platform.

Power Automate handles system logic and integrations.

---

# Flow 1 — Email → Task Creation

Purpose:

Automatically create tasks from important emails.

Trigger:

New email received in monitored inbox.

Process:

1. Read email subject
2. Capture sender
3. Extract task description
4. Create task in SharePoint

Output:

New task created in Tasks list.

---

# Flow 2 — Daily Scrum Carry Over

Purpose:

Move unfinished tasks to the next day.

Trigger:

Scheduled daily flow (end of day).

Process:

1. Identify tasks with status ≠ Completed
2. Update task due date
3. Register in Daily Scrum log

Output:

Pending tasks automatically carried forward.

---

# Flow 3 — Deadline Alerts

Purpose:

Notify responsible users of approaching deadlines.

Trigger:

Scheduled daily check.

Process:

1. Check tasks with due date within 24 hours
2. Send notification email

Output:

Deadline alert sent to responsible user.

---

# Flow 4 — Priority Alerts

Purpose:

Highlight critical tasks.

Trigger:

Task priority updated to Critical.

Process:

1. Detect priority change
2. Notify responsible
3. Add alert in dashboard

Output:

Critical task alert created.

---

# Flow 5 — Project Status Update

Purpose:

Automatically update project progress.

Trigger:

Task status changed.

Process:

1. Count completed tasks
2. Calculate project completion %
3. Update project record

Output:

Project progress automatically updated.
