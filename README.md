# 📊 NYC Small Business Data Analysis (ETL Project)

This project implements an end-to-end **ETL pipeline** using **SSIS (SQL Server Integration Services)** to analyze small business data in New York City, with a focus on **Women- and Minority-Owned Business Enterprises (WBE/MBE)**. It includes data transformation, dimensional modeling, SQL querying, and reporting.

---

## 📁 Project Files

### 🔧 SSIS Project Files
- `Project_PRJ.dtproj` – SSIS project definition
- `Project.dtsx` – ETL data flow and control flow
- `Project.params` – Project-level parameters
- `Project_PRJ.database` – Target database settings
- `Project_PRJ.dtproj.user` – User-specific project config (optional)

### 📄 Documentation & Reports
- `presentation.pptx` – Slide deck covering goals, workflow, results

### 🗃️ Data & Scripts
- `Introducing Keys.csv` – Source/raw data
- `SQLQuery48.sql` – Business case queries (WBE, MBE, borough-level filtering, contract ranking)

### 🖼️ Results
- `screenshots/` – Visual outputs and query result screenshots (to be uploaded)

---

## 🔄 ETL Workflow Summary

1. **Data Cleaning**:
   - Removed NULLs, duplicates, improper formats
   - Replaced malformed names and reformatted certifications

2. **Dimensional Tables**:
   - Created 3 dimension tables: Vendors, Contracts, Geographic Info

3. **Fact Table**:
   - Merged cleaned streams (VendorGeo + ContractVendor) into a centralized FACT table

4. **SQL Analysis**:
   - Identified WBE/MBE vendors
   - Analyzed by borough (e.g., Manhattan)
   - Ranked businesses by contract value

---

## 💻 Tools Used
- **SSIS** (SQL Server Integration Services)
- **SSMS** (SQL Server Management Studio)
- **Excel** (for early data inspection)
- **PowerPoint** (for presentation)

---

## 📸 Screenshots
Result images and SQL output examples are in the [`screenshots/`](./screenshots) folder.

---

## 🧠 Authors
**Vaishnavi Chintala**  
**Jashwanth Reddy Yelakonda**
