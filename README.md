# 📊 Marketing Lead Pipeline Dashboard

An exploratory data analysis and interactive dashboard built to help the marketing team better understand the current lead pipeline, identify conversion bottlenecks, and surface actionable opportunities.

---

## 📁 Project Overview

| Item | Detail |
|---|---|
| **Dataset** | `Sales_Lead_Dataset.xlsx` |
| **Notebook** | `Marketing_Lead_Pipeline_Dashboard.ipynb` |
| **Tools** | Python, Pandas, Plotly Express, Google Colab |
| **Total Leads Analyzed** | 401 |
| **Overall Enrollment Rate** | **72.8%** (292 enrolled) |

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas plotly openpyxl
```

### Running the Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/sy3977-tech/Marketing_Lead_Pipeline.git
   cd Marketing_Lead_Pipeline
   ```

2. Place `Sales_Lead_Dataset.xlsx` in the root directory.

3. Open the notebook:
   ```bash
   jupyter notebook Marketing_Lead_Pipeline_Dashboard.ipynb
   ```

   > **Google Colab users:** Upload both files to your Drive and mount it using the provided cell at the top of the notebook.

---

## 📈 Dashboard Visualizations

The notebook contains **5 interactive Plotly charts**, each paired with a key insight and recommended action:

### 1. Total Leads by Current Status
A bar chart showing the overall pipeline health and volume breakdown by lead status (Enrolled, No Response, Connecting, etc.).

> **Insight:** 292 leads are Enrolled, but 70 are stuck in "No Response" — the largest unconverted segment and the primary pipeline bottleneck.

---

### 2. Lead Status Distribution by Student Category
A stacked bar chart comparing conversion rates across four student demographics: Graduate, Undergraduate, OPT, and J1.

> **Insight:** Graduate students convert efficiently and at high volume. Undergraduate students, however, show a disproportionately high "No Response" rate — nearly half of all unresponsive leads.

---

### 3. Follow-Up Count Distribution vs. Lead Status
A box plot showing how many follow-up attempts were made for each lead outcome.

> **Insight:** Enrolled leads need an average of only **1.55 follow-ups**. "No Response" leads consume an average of **5.23 follow-ups** with zero return — a significant drain on sales resources.

---

### 4. Impact of Group Connection on Lead Outcome
A grouped bar chart comparing enrollment outcomes for leads with vs. without a group connection.

> **Insight:** Group-connected leads enroll at a **90.1% rate** (192/213), while non-connected leads drop to a **53.2% rate** and account for almost all "No Response" cases.

---

### 5. Weekly Lead Generation by Status
A line chart tracking lead volume and outcomes week by week to detect seasonal trends and campaign spikes.

> **Insight:** Enrollments occur in waves, with a major spike in **late August**. "No Response" rates also surge during this period, suggesting the sales team gets overwhelmed and leads fall through the cracks.

---

## 🧠 Executive Summary

The current lead pipeline demonstrates strong overall performance with a **72.8% enrollment rate** (292 out of 401 total leads). However, deeper analysis reveals clear opportunities to optimize sales resources and improve conversion for underperforming segments.

### Key Findings & Recommended Actions

**1. Group Connections Drive Conversions**
Leads connected to a group enroll at a 90.1% success rate vs. 53.2% for non-connected leads. Non-connected leads account for 59 of the 70 "No Response" cases.
- ✅ *Action:* Prioritize campaigns that generate group-affiliated leads. Redesign initial outreach so that joining a group is the clear, immediate next step for every new lead.

**2. Cap Manual Follow-Ups to Protect Sales Bandwidth**
High-intent leads enroll after ~1.55 follow-ups, while "No Response" leads absorb ~5.23 follow-ups with no conversion payoff.
- ✅ *Action:* Set a hard cap of 3–4 manual outreach attempts. After that threshold, automatically move unresponsive leads into a low-touch automated email nurture sequence.

**3. Adjust Messaging for Undergraduate Students**
Graduate students are the top-performing segment (105 enrollments). Undergraduates, however, make up nearly half of all "No Response" leads (34/70) despite being a high-volume segment.
- ✅ *Action:* Develop undergraduate-specific messaging that provides more introductory information or alternative incentives to reduce early-stage drop-off.

**4. Prepare Early for the Late August Rush**
Enrollment spikes sharply in late August (likely back-to-school), but "No Response" rates spike alongside it — indicating the team is unable to keep up with volume during peak periods.
- ✅ *Action:* Pre-schedule additional staffing and automated welcome sequences before the August surge to ensure no leads are lost due to capacity constraints.

**5. Re-Engage Stalled Leads**
93 leads are currently stalled: 70 in "No Response" and 23 in "Connecting."
- ✅ *Action:* Launch a targeted re-engagement campaign with a limited-time offer or incentive to push these warm leads across the finish line.

---

## 📂 Repository Structure

```
├── Marketing_Lead_Pipeline_Dashboard.ipynb   
├── Sales_Lead_Dataset.xlsx                  
└── README.md                                 
```

---

## 🛠 Tech Stack

- **Python 3**
- **Pandas** — data manipulation and aggregation
- **Plotly Express** — interactive visualizations
- **Google Colab** — development environment
- **OpenPyXL** — Excel file reading

---

## 📝 Notes

- The `Sales_Lead_Dataset.xlsx` file is **not included** in this repository. Place your own copy in the root directory before running the notebook.
- All visualizations are interactive (zoom, hover, filter) when run in a Jupyter or Colab environment.
