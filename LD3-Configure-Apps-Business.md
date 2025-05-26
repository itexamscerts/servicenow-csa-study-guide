## ✨ Bonus Study Tip

For those preparing for the ServiceNow CSA exam, we’ve tailored this entire guide to match **core exam competencies**. To gain hands-on exposure with scenario-style questions and preparation materials, check out our specialized CSA exam **[practice questions and dumps](https://www.itexamscerts.com/servicenow/csa-dumps.html)**.

# LD3: Configure Applications for Collaboration (20%)

## MD3.1: Configure Applications for Business – Lists, Filters, and Tags

### ✨ Knowledge: Classic List Views (\[SNAF Module 3.1])

* **How to access a List and what it represents:**

  * A List displays records from a table.
  * Found in Classic View (CV) application modules or Workspace (WS) landing pages.

* **Classic List - Context Menus (3 types):**

  * **List Control Menu:** view/filter options
  * **Column Options Menu:** configure/export/reporting
  * **Record Context Menu:** assign/filter/modify records

* **Filters & Quick Filters:**

  * Use show/hide filter icon or context menu shortcuts.
  * Filters consist of **Field, Operator, Value**.

* **Inline Editing & Multi-Edit:**

  * Shift-click or checkbox select multiple records.
  * Click column header > *Update Selected* to edit.

* **Quick-edit Functions (4):**

  * Assign to Me
  * Assign Tag
  * Approve / Reject (where applicable)

* **Configure List Layout:**

  * Column Options > Configure > List Layout
  * Use List Collector to add/remove/reorder fields.
  * Can change or create views, even new fields.

* **Dot-Walking:**

  * Add fields from related tables to a List View.

* **Required Role:** `personalize_list`

* **Application Menus:**

  * Add apps/modules via: All > System Definition > Application Menus

* **List Personalization:**

  * Use the gear icon on column header for personal customization.

* **Tags:**

  * Right-click a field > Assign Tag > New Tag

---

### 📝 Practice Tasks \[SNAF Lab 3.1 - Classic List Views]

* Navigate to: All > Incident > All > Configure > List Layout
* Create a new View; use List Collector and Dot-Walking.
* Save and verify from List Context Menu.
* Add a new Application Menu and Module.
* Set visibility and verify.

---

## List and Form Anatomy

### ✨ Knowledge: Views & Switching

* Views control field visibility/order.
* Switch via List Controls > View.
* Default sort: order, number, name, or table's display field.
* Some List Views are Workspace-bound but editable only in Classic View (e.g., SOW Landing Page).

---

## MD3.2: Create Workspace List Views

### ✨ Knowledge: Workspace Lists (\[SNAF Module 3.2])

* **List Viewing Modes:** Grid, List, New Tab
* **Context Menus:**

  * Grab Icon (move column)
  * More Options (group by column value)
  * Filter Actions (Show Matching / Filter Out)
* **List Filters:** Field, Operator, Value
* **Multi-Edit:** Shift-click/edit with *Edit (#)* > Update
* **Enable Inline Editing:** `glide.lists.inline_editing_enabled`
* **Configure WS Lists:**

  * Same as CV: Configure > List Layout
* **UI Builder:**

  * Create new Category and UX List
  * Use *Configuration Panel* > List Menu Configuration > UX Lists & Categories
* **Audience Applicability:**

  * UI Builder > View > M2M Applicability

---

### 📝 Practice Tasks \[SNAF Lab 3.2 - Workspace Lists]

* Update Incident List View in Service Operations Workspace
* Add new UX List Category in UI Builder
* Link to audience with M2M Applicability

---

## Forms

### ✨ Knowledge: Classic & Workspace Forms (\[SNAF Module 3.3])

* **Forms display fields for one record**
* **Classic View Anatomy:** Fields, Sections, Activity Stream, UI Actions, Related Lists
* **Workspace View Anatomy:** Details tab, grouped sections, activity panel

### Form Design vs Layout

* **Form Design:** Drag-and-drop interface
* **Form Layout:** List Collector with `-split-` indicators
* **Access via Header > Configure > Form Layout / Form Design**
* **Limitations of Design:** No dot-walking support

### Related Lists & Personalization

* **Configure Related Lists:** Header > Configure > Related Lists
* **Personalization:** Classic (gear icon) / Workspace (Details > jump-to-section)
* **Disable Personalization for itil:** `glide.ui.personalize_form.role = admin`

### Form Designer Components

* Page Header, Field Navigator, Form Layout
* Formatters = form elements for displaying non-record info

---

### 📝 Practice Tasks \[SNAF Lab 3.3 - Forms]

* Configure Form Layout on Incident
* Add/rearrange fields with List Collector
* Update Workspace view and verify via impersonation
* Edit New Record Form as well

---

## MD3.4: Advanced Form Configuration – Choice & Reference Lists

### ✨ Knowledge (\[SNAF Module 3.4])

* **Choice List:**

  * Add/remove options with *Configure Choices*
  * *Show Choice List* displays all values for that field

* **Reference List:**

  * Use magnifying glass icon to select referenced records

---

### 📝 Practice Tasks \[SNAF Lab 3.4 - Category/Reference Values]

* Create new Group for Incident Service Offering
* Configure Choices to add new Service
* Create Service & Service Offering records
* Assign groups to both records
* Impersonate ITIL user and verify availability & group auto-population

---


Continue exploring other modules and learning domains in the CSA certification path by visiting our [ServiceNow CSA Study Guide Hub](https://www.itexamscerts.com/servicenow/csa-dumps.html).
