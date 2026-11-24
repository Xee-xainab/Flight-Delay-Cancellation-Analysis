# Flight Delay & Cancellation Analysis (Excel Dashboard)

An interactive Excel dashboard that analyses 98,619 passenger flight records to understand where and when flight delays and cancellations happen, and whether passenger demographics play a role.

## Business Problem

Delayed and cancelled flights cost airlines revenue and passenger trust. This project identifies where and when disruptions occur so operations teams can focus on the fixes that matter most.

## Dataset

- 98,619 passenger flight records
- Fields: airport name, country, continent, month, flight status (On Time, Delayed, Cancelled), passenger gender, age group

## Tools

- Microsoft Excel (PivotTables, slicers, formulas, charts)

## Methodology

1. **Data preparation:** Reviewed columns, data types, duplicates, missing values and inconsistent text entries.
2. **Metrics defined:**
   - Delay rate = delayed flights / total flights
   - Cancellation rate = cancelled flights / total flights
   - Disruption rate = (delayed + cancelled) / total flights
3. **Grouping:** Age bands (Under 18, 18-30, 31-45, 46-60, 60+), months, airports, countries and continents.
4. **Summaries:** PivotTables for each view. Gender was compared using percentages because the groups differ in size.
5. **Dashboard:** Three linked pages (Overview, Disruption, Demographics) with slicers, KPI cards and charts.
6. **Validation:** 32,846 + 32,942 + 32,831 = 98,619 flights; monthly disruptions add up to 65,773.

## Dashboard Pages

| Page | What it shows |
|------|---------------|
| Overview | KPI cards, flight status, top 10 disrupted airports, monthly disruption |
| Disruption | Disruption by country and continent, delay, cancellation and disruption rates |
| Demographics | Flight status by gender and age group |

## Key Insights

- Only **33.3%** of flights were on time; **33.4%** were cancelled and **33.3%** were delayed (66.7% disrupted).
- Disruption is steady across the year, peaking in **May (5,699)** and lowest in **February (5,102)**.
- San Pedro Airport has the most disruptions (43), but the top 10 airports range only from 28 to 43, so no single airport dominates.
- By count, the United States and North America lead, mainly due to flight volume. By rate, every continent is within about 1 percentage point of 66.7%.
- Countries with the highest rates (Palau, Isle of Man, Sint Maarten) likely have very few flights and should be checked before being treated as problem areas.
- Flight status is almost equally split across genders (on-time: 33.4% male, 33.2% female) and age groups, so disruption does not depend on who the passenger is.

## Recommendations

- Review system-wide causes of cancellations and delays instead of targeting one airport, region or season.
- Prepare extra capacity ahead of May and August.
- Track disruption **rate** per country with a minimum flight count so small samples do not mislead.
- Give extra support (rebooking help, clear updates) to the largest passenger groups (60+ and Under 18) during disruptions.

## Limitations

- The dataset has no cause field (weather, technical, crew), so root causes cannot be confirmed.
- The almost perfect one-third split across statuses is unusual for real airline data, so results reflect patterns in this dataset.

## Files

- ## Files

- `dashboard_screenshots/`: images of the three dashboard pages
- [Download the Excel dashboard](https://docs.google.com/spreadsheets/d/1HKGFjF0JA0uUmQJztocZrEjM6Jdb0NuE/edit?usp=drive_link&ouid=110920329662697338984&rtpof=true&sd=true): hosted on Google Drive because of file size
- `Flight_Delay_Cancellation_Report.pdf`: 2-page report

## Author

**Zainab Danjuma**
