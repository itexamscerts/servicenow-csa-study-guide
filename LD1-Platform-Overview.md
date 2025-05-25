# LD1: Platform Overview & Navigation (7%)

> 🧠 This study guide summarizes the key areas tested in the CSA (Certified System Administrator) exam.
> 📘 Content is based on publicly available materials, ServiceNow learning paths, and student feedback.
> 📝 Ideal for last-minute review and reinforcing concepts that appear in real CSA exams.

🎯 Looking for updated CSA exam practice questions and dumps?
[👉 Click here for CSA Practice Questions – itexamscerts.com](https://www.itexamscerts.com/servicenow/csa-dumps.html)

---

## ServiceNow Platform Overview

### Modernized Work Experience

💡 **Knowledge \[Welcome to ServiceNow]:**

* Know both the founder and the CEO of ServiceNow
  **Founder:** Bill Luddy
  **CEO:** Bill McDermott
* Understand the capabilities of the platform (single system of record, single data model, configurable, plug ‘n play, etc.)
* Know the 4 ServiceNow workflows: IT Workflows, Customer Workflows, Creator Workflows, Employee Workflows
* Know the 4 ServiceNow interfaces:
  The Next Experience (Unified Navigation), Now Mobile App, Service Portal, Employee Center

### Useful Resources

💡 **Knowledge \[Welcome to ServiceNow]:**

* Know the 4 useful resources within this module:
  Now Learning, ServiceNow Community, Service Global Events, ServiceNow Developer Site

## Platform Capabilities & Services

### ITSM Incident Management

💡 **Knowledge \[SNAF Module 1 - Modernized Work Experience]:**

* Navigate to an Incident: `All > Incident > Create New`
* Understand Incident Lifecycle: New → In Progress → On Hold → Resolved → Closed → Canceled
* Understand Classic View functionalities: assigning fields, updating notes, viewing activity stream
* Assignment handling via groups/services, difference between **Work Notes** (internal) vs **Additional Comments** (visible to requester)
* Prioritization: Impact + Urgency = Priority (e.g., Impact 1 + Urgency 1 → Priority 1)
* Know what SLAs are and how they're reflected in Related Lists

📝 **Practice Style Example \[SNAF Lab 1.2]:**

* Impersonate Beth Anglin
* Create and assign an Incident
* Update Notes/Comments and access through "My Group’s Work"

### Service Operations Workspace

💡 **Knowledge:**

* Access via Top Header > Workspaces > Service Operations Workspace
* Understand dashboard widgets: Incidents, SLAs, Catalog Tasks, etc.
* Classic View mapping within Workspace layout
* Right-panel tools: Record Info, Agent Assist, Experts On-Call, Attachments, Templates
* Related Records and List View tree navigation

📝 **Practice Style Example \[SNAF Lab 1.3]:**

* Open incident in Workspace, explore layout, update notes/comments, resolve incident

### Employee Center Portal

💡 **Knowledge:**

* Access via: `All > Self-Service > Employee Center`
* Layout: My Tasks, Requests, Favorites, Knowledge, Search, Virtual Agent

📝 **Practice Style Example \[SNAF Lab 1.4]:**

* Impersonate Fred Luddy and Beth Anglin to track and update Incident requests

## The ServiceNow Instance

💡 **Knowledge:**

* Baseline Implementation = base install pre-config/customization
* Configuration vs Customization:
  Config (No-code), Custom (via scripts, plugins)
* Environment Types: Production, Non-Production (Dev, QA, UAT, etc.)
* Single-tenant architecture → isolated DB and customizations

## Next Experience Unified Navigation

### All Menu

📝 **Practice Tip:** Use filter (min. 2 chars) to find apps/modules

### Favorites / Pins

📝 Add/remove via star icon; pin/unpin in header tab

### History

📝 Learn what appears in history: records, not homepages/UI pages

### Workspaces

📝 Access: Top Header > Workspaces > Service Operations Workspace

### Elevation

💡 **Knowledge:**

* Elevate Role via User Menu > Elevate Role (red border/up arrow)
* Roles: `security_admin`, `workspace_admin`

### Impersonation

💡 **Knowledge:**

* Access via User Menu > Impersonate (red border/eye icon)
* Roles needed: `admin` or `impersonator`
* Test roles to create: `admin`, `ess`, `itil`
* System property: `glide.sys.log_impersonation`

📝 Impersonate to test user roles and log behavior

---

✅ **Pro Tip:** For updated CSA questions and practice tips, bookmark:
[https://itexamscerts.com/servicenow-csa](https://www.itexamscerts.com/servicenow/csa-dumps.html)
