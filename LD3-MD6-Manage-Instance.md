# LD3: Configure Applications for Collaboration (20%)  
## MD6: Manage an Instance

> 📘 **Get updated exam dumps and realistic practice questions at** 👉 [itexamscerts.com](https://itexamscerts.com) — your edge for CSA exam success!

---

### 📊 Performance Dashboard  
💡 *Knowledge* [SNAF Module 6.1 - Identify High Volume and Slowness Patterns]  

- Understand the importance of Change Management and its key stages:
  - Scheduling the change  
  - Recognizing blackout windows  
  - Coordinating changes to reduce conflicts  
- Change request lifecycle:
  - Creation & Scope → Approval → Implementation → Closure  
- Access the Performance Dashboard:  
  - **All > Self-Service > Dashboards**, select **ServiceNow Performance**  
- Base Performance Analytics architecture:
  - Available Graph Sets: `AMB`, `Database`, `Instance View`, `MySQL Global Status`, `ServiceNow Servlet`, `Slow Pattern`
  - Configure instance, timespan, and compare graphs  
  - Filter graphs by clicking categories  

📝 *Practice Tasks* [SNAF Lab 6.1]:  
- Open Performance Dashboard  
- Set Graph Set: `Instance View` → Timespan: `30 days`  
- Analyze `Transaction per Minute` and `Response Times`  
- Change to `ServiceNow Servlet` and identify `Network active threads`

---

### 🧪 System Diagnostics  
💡 *Knowledge* [SNAF Module 6.1]  

- Deprecated since San Diego release  
- Still remember `stats.do` for Stats Tools!

---

### 🧩 Instance Scan  
💡 *Knowledge* [SNAF Module 6.2 - Monitor an Instance]  

- Navigate via:  
  - **All > Instance Scan > Dashboard**  
  - Or **Self-Service > Dashboards**

- Understand Check types:  
  - `Table`, `Column Type`, `Script Only`, `Linter`  
  - Score `100 = Passed` (no finding), `<100 = Failing` (creates finding)

- Suites = Groups of checks  
- Result = scan outcome | Finding = record that violates a rule  
- Cleanup = Erases previous scan data

📝 *Practice Tasks* [SNAF Lab 6.2]:  
- Go to `Instance Scan > Suites`, select and run scan  
- Check scores, review `<100` failures  
- Click **Scan Findings** and investigate Resolution tips  
- Research Instance Scan vs. HealthScan vs. Troubleshooter

---

### ❤️‍🩹 Health Scan  
💡 *Knowledge* [SNAF Module 6.2]  

- Know that Health Scan exists  
- Optional: Watch YouTube overview

---

### 🌱 IT Adoption Journeys  
💡 *Knowledge* [SNAF Module 6.3 - Extending Value]  

- Access via **Admin > IT Adoption Journeys**  
- Explore platform features and Adoption Blueprints

---

### 🔄 Upgrades and Releases  
💡 *Knowledge* [SNAF Module 6.3 - Extending Value]  

- Use `docs.servicenow.com > Release Notes and Upgrades`  
- Understand:
  - **Family**: Major release group (e.g., Tokyo)  
  - **Upgrading**: Move to new family  
  - **Updating**: Apply patch/hotfix in same family  
- Know the 7 Phases of Upgrade:
  1. Read notes & plan
  2. Prep dev instance
  3. Schedule & verify
  4. Upgrade & validate dev
  5. Upgrade non-prod
  6. Prep for prod
  7. Upgrade prod  
- Access: `All > Upgrade Center`  
- Rollback window: 10 days via ServiceNow Support

📝 *Practice Tasks* [SNAF Lab 6.3]:  
- Navigate to Release Notes & Upgrades  
- Use **Build your own release notes**  
- Filter highlights, download as PDF  
- Review Upgrade Planning Checklist

---

> ✅ **Want more exam-focused dumps and laser-sharp CSA prep materials?** Dive in at 👉 [itexamscerts.com](https://itexamscerts.com) and get CSA-ready with confidence!

