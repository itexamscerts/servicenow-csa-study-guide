# LD6: Data Migration and Integration (15%)

## Client Scripts
💡 **Knowledge [SNAF Module 8.1 - UI Policies and Business Rules]**  
Client Script: Makes real-time changes to the appearance of the UI (esp. forms).  
**4 Types of Client Scripts:**
1. `onCellEdit()`
2. `onChange()`
3. `onLoad()`
4. `onSubmit()`

---

## UI Policies
💡 **Knowledge [SNAF Module 8.1]**

- **Script Language**: JavaScript  
- **Execution:**
  - Client-side: Web browser
  - Server-side: ServiceNow database

**UI Policy**: Rule applied to a form to dynamically change it.  
**3 UI Policy Actions:**
1. Mandatory / Optional  
2. Hidden / Visible  
3. Read-only / Editable

**Data Policy vs UI Policy**
- UI Policy: Only on form data  
- Data Policy: Enforced on all data platform-wide

**UI Actions** can run client or server side (based on client checkbox).  
**7 Typical UI Actions:**
- Form buttons, context menus, links  
- List buttons, context menus, choices, links

---

## 🧪 Practice Tasks (UI Policies & Business Rules)

### 1. Prepare Forms
- Add `Contact` to new **Company** form
- Add `Manufacturer` to **Service Offering**
- On **Incident** form:
  - Create `Escalate to manufacturer` (true/false)
  - Add `Manufacturer contact` field (Reference → User)

### 2. Prepare Data
- Create **Test Contact** user  
- Add company: **Infinity Products, Inc.**
- Add to **Infinity (HHD)** Service Offering

### 3. Create UI Policy
- Table: Incident  
- Conditions: `Priority = 1-Critical` & `Service Offering = Infinity (HHD)`  
- On load: ✅ | Reverse if false: ✅

### 4. UI Policy Actions
- Show `Escalate to manufacturer`
- Show `Manufacturer contact`

### 5. Verify
- Set Incident Priority to 1-Critical → fields appear  
- Change to non-critical → fields hide

---

## Business Rules
💡 **Knowledge [SNAF Module 8.1]**  
Business Rule runs when a record is displayed, inserted, updated, deleted, or queried.

**4 Configurations:**
1. Table  
2. When (timing)  
3. Conditions  
4. Actions  

**Catalog UI Policies** – can run on:
- `onLoad()`
- `onChange()`
- `onSubmit()`

### Practice Tasks
#### 6. Create Business Rules
1. **Escalate to Manufacturer reminder**  
   - Table: Incident  
   - Condition: Service Offering = Infinity (HHD) & Escalate = True  
   - Action: Show message

2. **Populate manufacturer contact name**  
   - Table: Incident  
   - Condition: Service Offering = Infinity (HHD) & Priority = 1-Critical  
   - Action: Populate Manufacturer contact field

#### 7. Verify
- Check field population and reminder message

---

## System Update Sets – Creating and Applying

### Creating
💡 **Knowledge [SNAF Module 8.2]**  
**Update Set**: Group of config changes to migrate between instances  
Includes:
1. Record details  
2. Change list  
3. State (In Progress / Complete)

**System Table**: `sys_update_xml`  
**Navigation**: `All > System Update Sets > Local Update Sets`  

**Note**:  
- Use batch sets to avoid wrong order or missing updates  
- Update Sets capture process records, not data  
- To export data: Use **Export XML**

### Practice Tasks
1. Review Default Global Update Set  
2. Create New Local Update Set  
   - Name: `Lab Update Set`  
   - Description: `Catalog item form, add Updated/Updated by fields`  
3. Modify Form (Infinity HHD Catalog Item)  
4. Verify updates in Lab Update Set

---

## Applying Update Sets

💡 **Knowledge [SNAF Module 8.3]**

### Steps to Apply:
1. Retrieve  
2. Preview  
3. Commit

**Navigation**:
- `System Update Sets > Retrieved Update Sets`  
- Use: **Import from XML**, Preview, then Commit  

**Fields to Match**: `sys_id`  
To update source or test connection:  
`Update Sources > Test Connection`

### Practice Tasks
- Mark Update Set as Complete  
- Export to XML  
- On another PDI: Import, Preview, Commit  
- Confirm changes on `Catalog Item > Hardware`

---

## ATF / App Engine Studio

### Automated Test Framework (ATF)
💡 Automate tests after instance changes.

**Benefits:**
- Faster dev & upgrade cycles  
- Clean test environments  
- Reuse tests, rollbacks, batch test suites

### App Engine Studio
Low-code tool for:
- Automating business processes  
- Empowering non-admin developers  
- Using templates for speed

**Designate Developers**: Non-admins with development permissions

---

## 🏁 CSA Exam Dumps & Practice Questions 2025

If you're preparing for the **CSA exam**, don’t miss out on the most up-to-date and accurate resources:

🎯 Download the latest [CSA exam dumps and practice questions (2025 edition)](https://www.itexamscerts.com/servicenow/csa-dumps.html)

These dumps are tailored to the **2025 CSA syllabus**, covering all 6 learning domains including:
- Data Migration & Integration  
- Client Scripts, UI Policies, Update Sets  
- ATF and App Engine Studio

### 🧠 Why Use These CSA Practice Questions?
- ✅ Verified by industry experts  
- ✅ Exam-style multiple choice & scenario-based  
- ✅ Covers real use cases from the ServiceNow platform

👉 [Get Your CSA Dumps 2025 Here](https://www.itexamscerts.com/servicenow/csa-dumps.html)

---
