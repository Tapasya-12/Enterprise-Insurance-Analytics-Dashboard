# 📊 Insurance Data Analysis Dashboard

*An end-to-end Power BI analytics solution for insurance policy, premium, and claims intelligence.*

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Published-brightgreen?style=for-the-badge)
![DAX](https://img.shields.io/badge/DAX-Data%20Modeling-blue?style=for-the-badge)

---

## 📌 Overview

The **Insurance Data Analysis Dashboard** transforms raw policy and claims records into a single, interactive Power BI report that helps stakeholders understand premium performance, claims behavior, and customer risk profiles at a glance.

Built on a dataset of **10,000+ policyholder records**, the report combines KPI cards, dynamic slicers, drill-through pages, and row-level security to deliver both a high-level executive summary and granular, policy-level detail — all in one governed, scheduled-refresh semantic model.

---

## 🎯 Objectives

- Consolidate scattered policy, premium, and claims data into one unified data model
- Track core business KPIs — **Premium**, **Coverage**, and **Claim Amounts** — in real time
- Break down claims by **status**, **policy type**, **age group**, and **customer activity**
- Enable self-service exploration through **slicers**, **drill-through**, and **cross-filtering**
- Ensure secure, role-based access via **Row-Level Security (RLS)** on the published semantic model
- Keep the report continuously up to date through **scheduled data refresh**

---

## 🖼️ Dashboard Preview

**Main Dashboard**

The landing page surfaces top-line KPIs alongside visual breakdowns of premium, claims, and customer segments.

| KPI | Value |
|---|---|
| 💰 Premium Amount | **5.98M** |
| 🛡️ Coverage Amount | **600.55M** |
| 📋 Claim Amount | **16.91M** |

**Key Visuals**
- **Premium Amount by Policy Type** — Travel leads at 2.5M, followed by Health, Auto, Life, and Home
- **Count of Active vs. Inactive Policies** — 58.13% Active vs. 41.87% Inactive
- **Number of Claims by Claims Status** — Rejected, Settled, and Pending claims tracked side by side
- **Claim Amount by Age Group** — Adults, Elder, and Young Adult segments compared
- **Gender-wise Policyholder Split** — Female vs. Male customer counts
- **Detailed Policy Type Table** — Pending, Rejected, and Settled amounts with running totals

**Data Table View**

A dedicated data view exposes the full transactional grain — Policy Number, Customer ID, Claim Number, Age, Gender, Coverage/Premium Amounts, Policy Start/End Dates, Policy Type, Claim Status, Claim Date, Age Group, and Active/Inactive flag — for granular auditing and drill-through.

---

## 🗂️ Dataset

| Attribute | Detail |
|---|---|
| **Source File** | `InsuranceData.csv` |
| **Records** | ~10,000 policy transactions |
| **Grain** | One row per policy/claim event |

**Key Columns**

| Column | Description |
|---|---|
| `PolicyNumber` | Unique policy identifier |
| `CustomerID` | Unique customer identifier |
| `Gender` | Policyholder gender |
| `Age` | Policyholder age |
| `PolicyType` | Auto, Health, Home, Life, Travel |
| `PolicyStartDate` / `PolicyEndDate` | Policy validity window |
| `PremiumAmount` | Premium paid on the policy |
| `CoverageAmount` | Total sum insured |
| `ClaimNumber` | Unique claim identifier |
| `ClaimDate` | Date the claim was filed |
| `ClaimAmount` | Amount claimed |
| `ClaimStatus` | Settled, Rejected, or Pending |
| `Age Group` *(calculated)* | Young Adult, Adults, Elder |
| `Active/Inactive` *(calculated)* | Policy activity status |

---

## ⚙️ Features & Techniques Implemented

- **Interactive Slicers** — Filter dynamically by Policy Number, Claim Number, and Customer ID
- **Drill-Through Pages** — Navigate from summary KPIs to detailed, policy-level views
- **Calculated Columns & Measures (DAX)** — Age Group segmentation, Active/Inactive flags, and aggregated KPI measures
- **Row-Level Security (RLS)** — Configured on the published semantic model to restrict data access by role
- **Scheduled Refresh** — Automated dataset refresh (232 rows tracked per cycle) to keep insights current
- **Cross-Filtering & Highlighting** — All visuals interact seamlessly for exploratory analysis
- **Published to Power BI Service** — Fully deployed report and semantic model, accessible via the Power BI workspace

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Report design, data modeling, DAX calculations |
| **Power Query (M)** | Data cleaning and transformation |
| **DAX** | Measures, calculated columns, KPI logic |
| **Power BI Service** | Publishing, scheduled refresh, RLS, sharing |

---

## 📈 Key Insights

- **Travel policies** generate the highest premium contribution (2.5M), nearly double that of Health policies
- **Rejected claims (4.4K)** outnumber both Settled (3.4K) and Pending (2.3K) claims — signaling a potential area for process review
- **Adults** account for the highest claim amount by age group (8.8M), followed by Elder and Young Adult segments
- The customer base is **near evenly split by gender** (5,001 Female vs. 5,003 Male)
- **58.13% of policies are Active**, indicating a healthy majority of in-force business

---

## 🚀 How to Explore

1. Open the `.pbix` file in **Power BI Desktop**, or view the published report directly on **Power BI Service**
2. Use the **slicers** at the top to filter by Policy Number, Claim Number, or Customer ID
3. Click any visual segment (e.g., a policy type bar or claim status slice) to **cross-filter** the entire report
4. Right-click a data point and select **Drill Through** to jump to the detailed record view
5. Data refreshes automatically on schedule — no manual updates required

---

## 🔮 Future Enhancements

- Add predictive claim-risk scoring using historical trends
- Introduce a fraud-flagging visual based on claim frequency and amount anomalies
- Expand RLS to support multi-tier regional access roles
- Build a mobile-optimized report layout

---

## 👩‍💻 Author

**Tapasya Patel**
B.Tech CSE, Nirma University

- GitHub: [Tapasya-12](https://github.com/Tapasya-12)
- LinkedIn: [patel-tapasya](https://linkedin.com/in/patel-tapasya)

---

*⭐ If you found this project useful or insightful, consider giving it a star!*
