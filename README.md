# AthleteX Care — Sports Injury Analytics Dashboard

**Power BI · DAX · Data Modelling · Healthcare Analytics**

A Data with Danny cohort project. You are a Data Analyst assigned to AthleteX Care — the medical and performance unit managing athlete health across multiple sports clubs, events, and regions. Leadership is making injury prevention decisions reactively, after athletes go down. Your dashboard changes that.

---

## The Scenario

AthleteX Care manages athlete health across multiple sports clubs, events, and regions. Medical staff are logging injuries at the club level, but leadership has no centralised way to:

- Monitor injury trends over time
- Identify which injury types are most expensive to treat
- Measure whether rehabilitation protocols are actually working
- Allocate prevention resources to the highest-risk groups

Decisions are being made reactively — after athletes go down — rather than proactively. Your job is to build the dashboard that changes that.

---

## Core Business Questions

| # | Question |
|---|----------|
| 01 | Are injury rates increasing or decreasing year over year, and which months are the most dangerous? |
| 02 | Which injury types cost the most to treat — and are those the same ones taking athletes the longest to recover from? |
| 03 | Are athletes returning to play on time, or are estimated recovery timelines consistently being missed? |
| 04 | Which age groups and genders carry the highest financial burden — should prevention resources be reallocated? |
| 05 | Is the reinjury rate high enough to suggest that current rehabilitation protocols are failing? |
| 06 | Which sport events and competition levels are producing the most severe and costly injuries? |

---

## Definition of Success

> The medical director can open the dashboard at the start of any week, select a year, and immediately know where the organisation stands on injuries, spend, and recovery — compared to the same period last year.
>
> Every insight needed to make an intervention decision is available within two clicks. No reports requested. No waiting.

---

## Your Deliverables

### 1. Injury Overview & Trend Analysis
Headline KPIs — total injuries, total treatment cost, average recovery days, reinjury rate. Monthly and yearly trend lines. Year-over-year comparison. Identify the most dangerous months.

### 2. Injury Type & Cost Analysis
Which injury types are most frequent? Which cost the most to treat? Are the most expensive injuries also the ones with the longest recovery times? Build a matrix that answers all three at once.

### 3. Recovery Performance Dashboard
Are athletes hitting their estimated return-to-play dates? Track actual recovery days vs estimated recovery days by injury type, age group, and treatment protocol. Flag where the system is consistently underestimating.

### 4. Athlete Risk Segmentation
Break down injury rates, treatment costs, and recovery performance by age group, gender, sport, and competition level. Surface which segments carry the highest financial and operational burden.

### 5. Reinjury & Protocol Effectiveness
Calculate reinjury rates by injury type and rehabilitation protocol. A high reinjury rate on a specific protocol is a signal that the protocol is failing. Surface it clearly.

### 6. Executive Summary Page
One-screen board-level view. This week vs same period last year. Top injury types by cost. Recovery adherence rate. Reinjury flag. Everything the medical director needs to make a decision in under 60 seconds.

---

## Dashboard Requirements

Your dashboard must include:

- [ ] Headline KPI cards — total injuries, total cost, avg recovery days, reinjury rate
- [ ] Year-over-year injury trend with monthly breakdown
- [ ] Injury type breakdown by frequency, cost, and recovery time
- [ ] Recovery adherence visual — estimated vs actual days
- [ ] Athlete segmentation by age group, gender, and sport
- [ ] Reinjury rate by protocol type
- [ ] Executive summary page — one screen, decision-ready
- [ ] Slicers for year, sport, club, injury type, and competition level
- [ ] Page navigation between views

---

## Data Model

Your star schema should include:

| Table | Type | Description |
|-------|------|-------------|
| fact_injuries | Fact | One row per injury incident |
| dim_athlete | Dimension | Athlete profiles — age, gender, sport |
| dim_injury_type | Dimension | Injury classification and severity |
| dim_treatment | Dimension | Treatment protocols and costs |
| dim_club | Dimension | Club and region |
| dim_event | Dimension | Sport events and competition level |
| dim_date | Dimension | Full date spine |

---

## Repository Structure

```
athletex-care-powerbi/
│
├── Dataset/
│   └── AthleteX_Injury_Data.xlsx       ← Connect Power BI here
│
├── Project Brief/
│   └── AthleteX_Business_Problem.pdf   ← Full brief
│
├── Dashboard/
│   └── AthleteX_Care_Dashboard.pbix    ← Your completed dashboard goes here
│
├── Report/
│   └── Medical_Director_Summary.pdf    ← Your executive summary goes here
│
└── README.md
```

---

## Success Criteria

- [ ] Data model built with correct relationships and a proper date table
- [ ] All 6 business questions answered in the dashboard
- [ ] Year-over-year DAX measures using time intelligence
- [ ] Reinjury rate calculated accurately in DAX
- [ ] Executive summary page passes the 60-second test
- [ ] The medical director persona can use this without training

---

## Tools Required

- Power BI Desktop (free)
- Microsoft Excel for the dataset

---

## How to Submit

1. Fork this repo or create your own public repo
2. Upload your completed `.pbix` file and executive summary
3. Update the README with your name, cohort number, and a screenshot of your dashboard
4. Share the link in the DwD community

**The goal is not just to complete the project. The goal is to build something you can show a recruiter or client.**

---

## Part of the DwD Curriculum

This is one of two Power BI projects in the **Data with Danny** cohort program — a structured 4-month curriculum covering Excel, SQL, Python, Power BI, Statistics, and AI integration.

**Cohort 9 starts June 25, 2026** → [nestuge.com/mzlik606d](https://nestuge.com/mzlik606d)

---

*Data with Danny · Power BI Project 2 · datawithdany@gmail.com*
