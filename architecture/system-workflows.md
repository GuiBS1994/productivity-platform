# System Workflows

This document describes the operational workflows of the Productivity Platform.

The workflows represent how users interact with the system and how data flows between components.

---

# Workflow 1 — Task Creation

User creates a task in Power Apps.

Flow:

User → Power Apps → SharePoint (Tasks List)

Steps:

1. User fills task form
2. Task saved in SharePoint
3. Task appears in Task list
4. Task becomes visible in Kanban board

---

# Workflow 2 — Email to Task

Important emails generate tasks.

Flow:

Outlook → Power Automate → SharePoint → Power Apps

Steps:

1. Email received
2. Flow triggered
3. Task created automatically
4. Task assigned to responsible user

---

# Workflow 3 — Project Management

Projects organize tasks.

Flow:

User → Power Apps → SharePoint

Steps:

1. Project created
2. Tasks linked to project
3. Project progress calculated
4. Dashboard updated

---

# Workflow 4 — Kanban Task Movement

Tasks move across workflow stages.

Flow:

Power Apps → SharePoint → Dashboard

Steps:

1. User drags task
2. Status updated
3. SharePoint updated
4. Metrics updated

---

# Workflow 5 — Daily Scrum

Daily operational meeting log.

Flow:

User → Power Apps → SharePoint → Power Automate

Steps:

1. Meeting registered
2. Pending tasks recorded
3. Tasks carried to next day if incomplete

---

# Workflow 6 — Operational Dashboard

Operational metrics visualization.

Flow:

SharePoint → Power Apps Dashboard

Metrics:

- Completed tasks
- Pending tasks
- Overdue tasks
- Active projects
