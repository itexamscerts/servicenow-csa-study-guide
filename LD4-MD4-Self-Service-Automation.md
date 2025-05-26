# LD4: Self Service and Automation (20%)

🔗 Looking for updated **ServiceNow CSA Dumps** and **exam practice questions**?  
Check out: 👉 [itexamscerts.com/servicenow/csa-dumps.html](https://www.itexamscerts.com/servicenow/csa-dumps.html)

---

## 📚 Knowledge Management

### Architecture
💡 **[SNAF Module 4.1 - Knowledge Management]**

- Centralized system to manage information across knowledge bases.
- Access: `All > Self-Service > Knowledge`
- Admin role required: `knowledge_admin`
- Setup: Use Guided Setup or manually via `All > Knowledge > Administration > Knowledge Base`
- Articles organized by categories; only one KB per article.

### User Criteria / Workflows
💡 **[SNAF Module 4.1]**

- Defines conditions for access:
  - `canRead`, `cantRead`, `canContribute`, `cantContribute`
- System Property:  
  `glide.knowman.block_access_with_no_user_criteria`
- Workflows:
  1. Approval Publish
  2. Approval Retire
  3. Instant Publish
  4. Instant Retire
  5. Publish Knowledge
  6. Retire Knowledge
- Word document import supported.
- Accessible in Now Mobile under: `All > Now Mobile App > Knowledge Bases`

### 🧪 Practice Tasks (SNAF Lab 4.1)

- Create new KB & user group with `knowledge_admin` + `approver_user`
- Assign Owner and Workflows
- Test User Criteria visibility by impersonation

---

## 📦 Service Catalog

💡 **[SNAF Module 4.2 - Create a Catalog Item]**

- Access: `All > Self-Service > Service Catalog`
- Role: `catalog_admin`
- Use Catalog Builder: `All > Service Catalog > Catalog Builder`

### Request Flow

- Creates: REQ (Request), RITM (Item), SCTASK (Task)
- Item components:
  1. Catalog Items
  2. Variables
  3. Variable Sets
  4. Record Producers
  5. Flows

- Record Producer → creates Task records
- Order Guide → bundles related items
- Tables:
  - REQ: `sc_request`
  - RITM: `sc_req_item`
  - SCTASK: `sc_task`

- Statuses: Waiting for Approval, Request Approved, Completed

### 🧪 Practice Tasks (SNAF Lab 4.2)

- Create Catalog Item with at least 3 questions using Catalog Builder
- Assign `catalog_admin` to user
- Preview > Submit > Maintain Items > Edit Price
- Test access restrictions with User Criteria

---

## ⚙️ Flow Designer

💡 **[SNAF Module 4.3 - Flow Designer]**

- Access: `All > Process Automation > Flow Designer`
- Roles:
  - `flow_designer`
  - `flow_operator`
  - `action_designer`

### Components

- 3 Triggers: Record-based, Date-based, Application-based
- 4 Flow Components: Triggers, Conditions, Actions, Data
- Common Actions: Ask for Approval, Create/Delete/Lookup Record, Wait for Condition
- Use Data Pill Picker (dot-walking supported)

### 🧪 Practice Tasks (SNAF Lab 4.3)

- Create Flow for a Catalog Item with:
  - Trigger: Catalog
  - Actions: Update RITM, Create Task, Send Email, Update REQ
- Activate and associate Flow
- Test impersonation and approvals

---

## 🤖 Virtual Agent

💡 **[SNAF Module 4.3 - Flow Designer]**

- Conversational platform in messaging UI
- Automates:
  1. FAQs
  2. How-to guides
  3. Record updates
  4. Data gathering
  5. Diagnostics
  6. Problem resolution
  7. File management

---

🔗 For verified **CSA dumps and updated exam practice** – get prepped the smart way!  
Visit: 👉 [itexamscerts.com/servicenow/csa-dumps.html](https://www.itexamscerts.com/servicenow/csa-dumps.html)
