# Bellabeat Wellness Case Study — Smart Device Usage Analysis
## How Can a Wellness Company Play It Smart?

# Project Overview
Bellabeat, a wellness technology company, wanted to understand how consumers use smart devices—particularly Fitbit trackers—to inform marketing strategy for its product line.
Using Fitbit data from 30 users, this project builds a complete analytical pipeline:
* Raw data ingestion
* Structured cleaning using BigQuery SQL
* Semantic‑layer modeling (M1 → M2 → M3)
* Trend analysis across daily, hourly, minute‑level, and sleep data
* Dashboard development using Google Connected Sheets
* Actionable marketing recommendations
  
This case study demonstrates how raw sensor data can be transformed into business intelligence that supports product positioning, user engagement, and holistic wellness strategy.

# Repository Structure
├── README.md
├── Capstone Project - Bellabeat Case Study.pdf
├── dashboards/
│   ├── daily_activity_dashboard.png
│   ├── hourly_activity_dashboard.png
│   ├── minute_wide_dashboard.png
│   ├── minute_level_dashboard.png
│   ├── sleep_dashboard.png
│   └── user_summary_dashboard.png
├── sql/
│   ├── m1_raw_layer.sql
│   ├── m2_clean_layer.sql
│   ├── m3_semantic_layer.sql
│   └── cleaning_workflow.sql
└── appendix/
    ├── appendix_a_dashboards.pdf
    └── appendix_b_data_dictionary.pdf

# Business Task
Bellabeat wants to identify behavioral trends in smart‑device usage to guide marketing strategy for one of its products (Leaf, Time, Spring, Bellabeat App).

## Key questions:
* What trends exist in smart‑device usage?
* How do these trends apply to Bellabeat customers?
* How can these insights shape Bellabeat’s marketing strategy?

# Dataset
* Source: Fitbit Fitness Tracker Data (Kaggle, CC0 Public Domain)
* Users: 30
* Period: April–May 2016
* Files: dailyActivity, sleepDay, dailySteps, dailyIntensities, heartrate_seconds, weightLogInfo, hourly tables, minute‑level tables.
  
## ROCCC Assessment
* Reliable: Partially (small sample size)
* Original: Yes
* Comprehensive: Limited (no demographics)
* Current: No (2016)
* Cited: Yes

# Tools & Technologies
* BigQuery SQL — data cleaning, transformation, semantic modeling
* Google Connected Sheets — dashboard creation
* Google Docs — documentation
* Python (optional) — validation and exploration

# Data Engineering Pipeline (M1 → M2 → M3)
## M1 — Raw Layer
* Original Fitbit CSVs
* Preserved schemas and naming conventions
## M2 — Clean Layer
* Duplicate removal
* Date format standardization
* Column normalization (snake_case)
* Missing value checks
* User ID consistency checks
* Merging daily, hourly, minute‑level, sleep, and weight tables
## M3 — Semantic Layer
Purpose‑built analytical tables:
* M3_daily_master
* M3_hourly_master
* M3_minuteWide_long
* M3_minute_master
* M3_sleep_master
* M3_user_summary
These tables power all dashboards and trend analysis.

# Key Insights Identified
## 1. Daily Activity Patterns
* Average steps: 7,000–8,000 (below recommended 10,000)
* Strong step–calorie correlation
* Weekend activity drop
## 2. Hourly Movement
* Long inactivity windows
* Intensity peaks align with HR spikes
## 3. Minute‑Level Behavior
* Micro‑patterns of movement
* METs reveal workout peaks and recovery periods
## 4. Sleep Duration & Efficiency
* Average sleep: ~6.9 hours
* Users spend more time in bed than asleep
* Irregular sleep patterns
## 5. User Wellness Profiles
* Moderate activity
* Irregular sleep
* Sparse weight/HR data

# Dashboards Created
Six dashboards were built using Google Connected Sheets:
* ## Daily Activity Dashboard
* ## Hourly Activity Dashboard
* ## Minute‑Wide Dashboard
* ## Minute‑Level Dashboard
* ## Sleep Dashboard
* ## User Summary Dashboard
Each dashboard includes multiple charts (line, scatter, histogram, heatmap, stacked bar).

# Marketing Recommendations
## 1. Promote Habit‑Building Features
* Daily step goals
* Weekend reminders
* Streak tracking
* Achievement badges
## 2. Highlight Sleep‑Tracking & Wellness Insights
* Sleep duration & quality
* Bedtime reminders
* Stress‑reduction tools
* Personalized sleep plans
## 3. Position Bellabeat as a Holistic Wellness Ecosystem
* Activity + sleep + stress + hydration + women’s health
* Bellabeat Membership Program
* Nutrition & mindfulness guidance

## 📄 Full Case Study
You can read the complete case study here:
👉 [Capstone Project – Case Study 2 – How Can Wellness Companies Play It Smart?](https://docs.google.com/document/d/1d7gHQhaKGOkKQR9asCschx2RKWH0e5AjrFvPcTeiIuE/view)

## Contact
If you’d like to discuss this project or collaborate:
* Author: Reyal Osman 
* Location: Abu Dhabi, UAE
* LinkedIn: (https://www.linkedin.com/in/reyal-osman-15a048221)
* GitHub:(https://github.com/reyalosman-m3/bellabeat-wellness-m3-case-study)

## Related Work
* Semantic Layer SQL
* Dashboard Design Guide
* Portfolio Formatting


