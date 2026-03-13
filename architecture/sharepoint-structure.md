# SharePoint Data Structure

This document defines the SharePoint Lists used by the Productivity Platform.

Each list represents a core entity of the system.

---

# List: Users

Stores all system users.

Fields:

- Name
- Email
- Department
- Role

---

# List: Projects

Stores all active projects.

Fields:

- ProjectName
- Description
- Owner
- Status
- StartDate
- EndDate

Status options:

- Planned
- Active
- On Hold
- Completed

---

# List: Tasks

Stores operational tasks.

Fields:

- TaskTitle
- Description
- Responsible
- Priority
- Status
- DueDate
- Project (Lookup)

Priority options:

- Low
- Medium
- High
- Critical

Status options:

- Pending
- In Progress
- Blocked
- Completed

---

# List: Daily Scrum

Stores daily meeting logs.

Fields:

- Date
- Team
- Notes
- PendingTasks

---

# List: Email Tasks

Tasks created from email follow-ups.

Fields:

- Subject
- Sender
- Responsible
- Status
- DueDate
