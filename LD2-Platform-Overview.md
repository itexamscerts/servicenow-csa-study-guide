# LD2: Instance Configuration (11%)

Explore how to personalize, configure, and control access in your ServiceNow instance, a core domain of the [ServiceNow CSA Exam](https://www.itexamscerts.com/servicenow/csa-dumps.html).

## 🔧 Personalizing / Customizing the Instance

### 💡 Knowledge – SNAF Module 2.1
- **Update the Company Logo**  
  Navigate: All > System Properties > My Company

- **Change Company Name**  
  Navigate: All > User Administration > Companies

- **Edit Browser Tab Title (Context Pill)**  
  Navigate: All > System Properties > System → Update Browser tab title to DEV

- **Enable Dark Theme**  
  Update property `glide.ui.polaris.dark_themes_enabled = TRUE` via sys_properties.list

### 📝 Practice Tasks – SNAF Lab 2.1: Configure an Instance
- Update company logo
- Change company name
- Modify browser tab title
- Enable the dark theme

---

## 📦 Installing Applications and Plugins

### 💡 Knowledge – SNAF Module 2.2
- **Access System Applications**  
  Navigate: All > System Applications > All Available Applications > All

- **Access Plugins**  
  Navigate: All > System Definition > Plugins

### Key Concepts
- Use [docs.servicenow.com](https://docs.servicenow.com) to research apps/plugins
- Understand licensing, dependencies, and demo data usage
- Application Scoping protects data/files from external apps

### 📝 Practice Tasks – SNAF Labs 2.2 - 2.3
- Use documentation to find required plugins
- Install with demo data in a non-prod instance

---

## 👥 Users / Groups / Roles

### 💡 Knowledge – SNAF Module 2.4
**5 Persona Types:**
- **System Administrator** – Access to most of the platform
- **Specialized Administrator** – Limited to specific apps (e.g., HR)
- **Process User** – Holds specific functional roles (e.g., itil)
- **Approver** – Can approve/modify approvals
- **Requester** – Submits/manages their own requests

### System Tables
- **Users** → sys_user
- **Groups** → sys_user_group
- **Roles** → sys_user_role

### Modify Access
- Navigate: All > User Administration > Users
- Navigate: All > User Administration > Groups
- Navigate: All > User Administration > Roles  
  OR: All > System Security > Users and Groups > *

### Role Hierarchies & Best Practice
- Assign roles to Groups, then assign Users to Groups

### 📝 Practice Tasks – SNAF Lab 2.4: Grant Access to Applications
- Create a user
- Assign user to a group
- Assign roles to the group

---

## 🧭 Common User Interfaces in the Platform

### 💡 Knowledge – Welcome to ServiceNow
**UI Elements:**
- Lists
- Forms
- Tasks
- Dashboards
- Reporting
- Workspaces
- Knowledge
- Service Catalog
- Virtual Agent

---

👉 For complete CSA preparation including practice questions and mock dumps, visit our CSA study hub:  
[CSA Practice Questions – itexamscerts.com](https://www.itexamscerts.com/servicenow/csa-dumps.html)

