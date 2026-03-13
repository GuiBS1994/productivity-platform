# Data Model — Productivity Platform

This document defines the core data structure used by the Productivity Platform.

The system uses SharePoint Lists as the primary data storage.

---

# Core Entities

## Users

Represents system users.

Fields:

- UserID
- Name
- Email
- Department
- Role

---

## Projects

Represents strategic or operational projects.

Fields:

- ProjectID
- ProjectName
- Description
- Owner
- Status
- StartDate
- EndDate

---

## Tasks

Represents operational tasks.

Fields:

- TaskID
- TaskTitle
- Description
- Responsible
- Priority
- Status
- DueDate
- ProjectID

---

## Daily Scrum Logs

Stores daily meeting notes.

Fields:

- ScrumID
- Date
- Team
- Notes
- PendingTasks

---

## Email Tasks

Tasks generated from email follow-ups.

Fields:

- EmailTaskID
- Subject
- Sender
- Responsible
- Status
- DueDate

---

# Relationships

Projects → Tasks (1:N)

Users → Tasks (1:N)

Users → Projects (1:N)

Tasks → Daily Scrum (optional reference)
