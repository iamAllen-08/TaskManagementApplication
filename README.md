# TaskManagementApplication

A simple and collaborative Task Management App designed to help teams create, assign, and track tasks with deadlines and statuses. Built using Agile methodology with clear roles and responsibilities.

---

##  Project Scope
- **In Scope (must-have features):**
  - Create, edit, delete tasks
  - Assign tasks to team members
  - Set deadlines and track status (Pending, In Progress, Completed)
  - Dashboard to view tasks

- **Out of Scope (future enhancements):**
  - Push notifications
  - Advanced analytics (charts, reports)
  - Integration with external tools (Slack, email)

---

##  Requirements

### Functional Requirements
- User can log in and manage tasks
- User can filter tasks by status or assignee
- System stores tasks persistently (local DB or cloud)

### Non-Functional Requirements
- App should load within 2 seconds
- UI should be responsive (desktop + mobile)
- Secure authentication for user login

---

## Team Roles

| Role           | Scope                          | Responsibilities                          | Example User Stories |
|----------------|--------------------------------|-------------------------------------------|----------------------|
| **Product Owner** | Define features, backlog       | Prioritize tasks, maintain requirements   | As a user, I want to create tasks with deadlines |
| **Scrum Master**  | Ensure Agile process           | Facilitate sprints, remove blockers       | As a team member, I want smooth sprint meetings |
| **Stakeholder**   | Provide feedback               | Review deliverables, ensure usability     | As a manager, I want reports of completed tasks |
| **Developer**     | Build features                 | Code CRUD operations, wireframes, testing | As a user, I want to add/edit/delete tasks |

---

## User Story Backlog
- As a user, I want to create tasks with deadlines so I can track my work.
- As a manager, I want to assign tasks to team members so responsibilities are clear.
- As a user, I want to mark tasks as complete so I can see progress.
- As a user, I want to filter tasks by status so I can focus on pending work.
- As a customer, I want to see task progress so I know work is on track.

---

##  SDLC Model
- **Chosen Model:** Agile (Scrum)
- **Reason:** Allows iterative development, feedback-driven improvements, and small deliverables per sprint.

---

##  Workflow Diagram & Wireframe
- Workflow: Requirements → Design → Development → Testing → Deployment → Review
- Wireframe: Simple dashboard with task list, “Add Task” button, and task cards showing title, assignee, deadline, and status.

---

##  Prototype / Feature
- Initial feature: **Add Task**
  - Form with Task Title, Deadline, Assignee
  - Save task in local storage or database
  - Display task in task list

---

##  Testing
- Test Cases:
  - Add task → Verify it appears in list
  - Edit task → Verify changes saved
  - Delete task → Verify removal
- Defects recorded in task board (GitHub Issues / Trello)

---

##  Deliverables
- README.md (this document)
- Requirements document
- Task board (backlog + sprint tasks)
- Workflow diagram + wireframe
- Prototype/feature code
- Test results document
- Presentation slides/demo

---

##  Team Retrospective
- **What went well:** Collaboration, clear role distribution
- **What didn’t go well:** Requirement clarity at start
- **Improvements:** Better sprint planning, more detailed user stories

## Test Cases

| Test Case ID | Feature          | Steps                                                   | Expected Result                          | Status |
|--------------|------------------|---------------------------------------------------------|------------------------------------------|--------|
| TC01         | Login            | Enter valid email + password → click Login              | User is redirected to Dashboard           | Pass   |
| TC02         | Login            | Enter invalid credentials → click Login                 | Error message “Invalid login”             | Pass   |
| TC03         | Add Task         | Fill form (title, deadline, assignee) → click Save      | Task appears in task list                 | Pass   |
| TC04         | Edit Task        | Select task → change title → Save                       | Updated task displayed                    | Pass   |
| TC05         | Delete Task      | Select task → click Delete                              | Task removed from list                    | Pass   |
| TC06         | Filter Tasks     | Select “In Progress” filter → Apply                     | Only tasks with status “In Progress” shown| Pass   |
| TC07         | Persistent Storage | Refresh page after adding task                         | Task still exists (stored in DB/file)     | Pass   |

##  Defect Log

| Defect ID | Description                | Steps to Reproduce                          | Severity | Status |
|-----------|----------------------------|---------------------------------------------|----------|--------|
| D01       | Task not saving            | Add task → refresh → task disappears        | High     | Open   |
| D02       | Filter not clearing        | Apply filter → click Clear Filters → tasks still filtered | Medium   | Open   |
| D03       | Login button misaligned    | On mobile view, button overlaps input field | Low      | Open   |
