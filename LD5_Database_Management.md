# LD5: Database Management (27%)

🌐 Visit: [itexamscerts.com](https://itexamscerts.com) for more ServiceNow CSA resources and practice!

---

## 📦 Data Schema

### 💡 Knowledge ([SNAF Module 7.1 - Data Schema])
- **3 Elements of the ServiceNow Infrastructure:**
  1. Tables
  2. Records
  3. Fields
- **Access System Dictionary:**  
  `All > System Definition > Dictionary` (Records are identified by `sys_id`)
- **Access Tables & Columns:**  
  `All > System Definition > Tables & Columns`
- **3 Key Field Attributes:**
  - Name
  - Label
  - Value
- **Reference Field:**  
  Stores `sys_id` of a record on another table (e.g. Caller references User table)

---

## 🔁 Relationships

### 💡 Knowledge ([SNAF Module 7.1 - Data Schema])
- **4 Table Relationship Types:**
  1. One-to-many
  2. Many-to-many
  3. Database View
  4. Extensions
- **One-to-Many Relationship Fields:**
  - Reference  
  - Glide List  
  - Document ID  
- **Inheritance Concepts:**
  - **Parent**: table being extended from  
  - **Child**: inherits all parent fields
- **Table Types:**
  - **Base**: can have children, no parent
  - **Core**: OOTB, can be parent/child
  - **Custom**: admin/dev-created
- **Namespace Identifiers:**
  - `_u`: Unscoped (global)
  - `_x`: Scoped

---

## 🗺 Schema Map

### 💡 Knowledge ([SNAF Module 7.1])
- **Access Path:**  
  `All > System Definition > Tables > Show Schema Map`

### 📝 Practice Task: Create Table for HHD Records
- Table: `u_cmdb_ci_hardware_hhd`, extends: `cmdb_ci_hardware`
- Add module: HHD → Configure view, create new field via Form Layout
- Add "Create New" module to Application Menu

---

## 🔐 Application / Access Control

### 💡 Knowledge ([SNAF Module 7.2])
- **3 Security Layers:**
  1. User Authentication
  2. Module Access (Roles)
  3. Database Access (ACLs)
- **Admin Security Modules:**
  - `System Properties > Security`
  - `System Security > Access Control`
  - `System Security > High Security Settings`
- **Access Control (ACL):**
  - Security rule to restrict data visibility/interactions
  - Set at record or field level
- **Access ACLs via:**  
  `All > System Security > Access Control (ACL)` (Requires `security_admin`)
- **Access Control Definition:**
  1. Operation
  2. Object
  3. Permissions
- **Default ACLs for Custom Table:**
  - Create, Read, Write, Delete + default role
- **ACL Rule Types:**
  - `table.none`, `table.field`, `table.*`
- **Best Practices:**
  - Use `table.none` with `.*` for clearer control logic

### 📝 Practice Tasks: Access Controls
- Assign and verify `u_holographic_handheld_hhd_user` role
- Limit visibility to Modules
- Grant roles to Support Groups
- Impersonate users to test restrictions
- Create and configure Incident ACLs with conditions
- Create `u_hhd_asset_tagger` role and ACL for `Asset Tag`
- Validate access based on impersonated user

---

## ⬇️ Importing Data

### 💡 Knowledge ([SNAF Module 7.3])
- **Import Set:**  
  Used to bring in data and map it to ServiceNow tables
- **5 Supported Data Sources:**
  - CSV, XML, Excel, JDBC, HTTP/FTP
- **Import Set Table:** Staging area  
- **Transform Map:** Moves data to target table
- **Mapping Utilities:**
  - Auto Mapping
  - Mapping Assist
- **Coalesce (De-duplication):**
  1. Single-field
  2. Multiple field
  3. Conditional (via script)

### 📝 Practice Tasks: Import Data
- Create `Import Validation` view
- Load `infinity_HHD-data.xlsx`, verify 7 records
- Create Transform Map (Auto Map + Mapping Assist)
- Load update file `infinity_HHD-updates.xlsx`, use coalesce
- Verify 19 total records exist
- Cleanup import set tables (`u_hhd_imports`)

---

## 🧠 CMDB and CSDM

### 💡 Knowledge ([SNAF Module 7.4 - CMDB])
- **CMDB Key Tables:**
  - `cmdb`, `cmdb_ci`, `cmdb_rel_ci`
- **CMDB Workspace:**
  View health, activity, dashboards
- **Configuration Item Form:**  
  - CI Attributes, CI Relationships
- **CI Class Manager Access:**  
  `All > Configuration > CI Class Manager`
- **Attribute Tabs:**
  - All, Derived, Added
- **CI Relationship Editor:** Related Items toolbar

### 📝 Practice Tasks: Explore CMDB
- Show Schema Map for HR Case, HHD table
- Pin Service & HHD in CI Class Manager
- Add "Runs on" relationship to Business Service
- Associate HHD devices to Service Offering (Infinity)
- View Legacy CI Relations
- Create Incident with HHD CI and verify hierarchy

---

## 🔧 CSDM

### 💡 Knowledge ([SNAF Module 7.4 - CMDB])
- **CSDM = Common Service Data Model**
- **Defines:**  
  - Standard CMDB data terms  
  - Best practices, core tables, service modeling, mappings
- **Does NOT Define:**  
  - Processes, reports, SKUs, implementations
- **Benefits:**  
  - Standardized offerings  
  - Reduced overhead  
  - Enables product/service consistency

---

## 🌐 Discovery & Service Mapping

### 💡 Knowledge ([SNAF Module 7.4])
- **Discovery:**
  - Inventories devices and apps, updates CMDB
- **Service Mapping:**
  - Adds IT dependencies between CIs
- **Mapping Types:**
  - **Top-down**: CI-to-service relationships
  - **Horizontal**: Inventory without dependencies

---

## 🔍 Dependency View

### 💡 Knowledge ([SNAF Module 7.4])
- **Visualizes upstream/downstream relationships**
- **Benefits:**  
  - Improved Incident, Change, and Problem Management

---

📘 For more deep dives and exam tips, visit: [itexamscerts.com](https://itexamscerts.com)
