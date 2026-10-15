# IndiGo Airlines — 5-Year Performance Overview

## Project Overview

This project is an interactive **Power BI dashboard** designed to analyse IndiGo Airlines' performance across a five-year period. It brings together flight operations, financial performance, load factor, passenger behaviour, customer satisfaction, and aircraft performance in one report.

The dashboard is organised into four analytical areas:
1. Overall Performance Overview
2. Flight Load Factor & Performance Analysis
3. Passenger & Customer Satisfaction Analysis
4. Aircraft Performance Analysis


### 1. Overall Performance Overview

The overview page presents headline KPIs and trends for the airline.

**KPI cards shown**
- Total Flights: 20K
- Total Passengers: 20K
- Total Profit: 5.32bn
- Total Operating Cost: 11.05bn

**Visuals**
- Flight Status Distribution (2021–2025)
- Monthly Load Factor Trend
- Annual Flight Operations Trend

**Purpose**
- Review high-level operational and financial indicators.
- Explore monthly load factor changes.
- Observe annual flight-operation trends across the displayed period.

### 2. Flight Load Factor & Performance Analysis

This page focuses on load factor by route and aircraft model.

**KPI shown**
- Average of `load_factor`: 74.42

**Visuals and controls**
- Route-wise Flight Performance table
- Load Factor by Route bar chart
- Load Factor by Aircraft Model bar chart
- Origin airport ID slicer
- Destination airport ID slicer
- Aircraft model filter

**Purpose**
- Compare load factor across routes and aircraft models.
- Review passenger totals and seat-capacity figures in the route table.
- Filter the report by origin and destination airport IDs.

**Data validation note:** The table displays `Sum of load_factor`. If `load_factor` is already a percentage or ratio, confirm that summing it is appropriate. An average or weighted calculation may be more meaningful depending on how the source data is structured.

### 3. Passenger & Customer Satisfaction Analysis

This page explores booking channels, gender distribution, ticket class, and satisfaction metrics.

**Visuals**
- Passengers by Booking Channel
- Customer Satisfaction by Booking Channel
- Passenger Distribution by Gender
- Ticket Fare vs. Satisfaction Score
- Customer Satisfaction by Ticket Class
- Passenger Distribution by Ticket Class

**Purpose**
- Compare passenger counts across booking channels.
- Compare average satisfaction scores across booking channels and ticket classes.
- Explore passenger distribution by gender and ticket class.
- Inspect the relationship between ticket fare and satisfaction score.

**Interpretation note:** Visual patterns are descriptive. They do not by themselves prove that ticket fare, gender, booking channel, or ticket class causes a change in satisfaction.

### 4. Aircraft Performance Analysis

This page compares aircraft models across financial and operational measures.

**Visuals**
- Revenue Contribution by Aircraft Model
- Profitability by Aircraft Model
- Operating Cost by Aircraft Model
- Passenger Distribution by Aircraft Model
- Flight Operations by Aircraft Model

**Purpose**
- Compare revenue and operating cost by aircraft model.
- Explore the profitability measure used in the report.
- Compare passenger distribution and flight-operation counts across aircraft models.

**Data validation note:** Confirm the definition and units of the profitability measure, and compare cost with revenue, passenger volume, and flight counts before drawing conclusions about aircraft efficiency.

## Tools & Technologies

- **Microsoft Power BI** — dashboard creation, KPI reporting, and data visualisation
- **Power Query / DAX** — include these only if they were used in the project

## Key Features

- KPI cards for flights, passengers, profit, and operating cost
- Five-year flight-operation trend
- Monthly load factor analysis
- Route and aircraft-model comparisons
- Booking-channel and customer-satisfaction analysis
- Ticket fare versus satisfaction scatter chart
- Passenger distribution by gender and ticket class
- Airport ID and aircraft-related filtering
- Consistent IndiGo-inspired blue dashboard theme

## Important Validation Checks

Before presenting business conclusions, verify the following in Power BI:

1. Confirm the definition of **Total Passengers** (for example, passenger records, bookings, or passengers flown).
2. Validate the DAX measures for **Total Profit**, **Total Operating Cost**, and revenue.
3. Check the units and aggregation used for `load_factor`, especially the route table's `Sum of load_factor`.
4. Confirm that the **Flight Status Distribution** title matches its plotted measure and axis labels.
5. Verify all KPI values and chart data directly against the source data.

The load-factor formula is commonly expressed as:

`Load Factor (%) = Passengers Flown / Available Seats × 100`

Use this formula only if the source fields represent passengers flown and the corresponding available seats for the same flights or period.

## How to Open the Project

1. Download or clone this repository.
2. Install Microsoft Power BI Desktop.
3. Open the `.pbix` file in Power BI Desktop.
4. If prompted, update data-source paths or credentials.
5. Refresh the data if the source files and required connections are available.
6. Use the report filters and visuals to explore the dashboard.

## Dashboard Screenshots

Add the actual exported dashboard screenshots to an `images` folder in this repository and update the filenames below if needed.

### Overall Performance Overview
<img width="894" height="504" alt="Screenshot 2026-10-15 211509" src="https://github.com/user-attachments/assets/45fcf844-e64d-42a7-b78b-926eb216b4d4" />


### Flight Load Factor & Performance Analysis
<img width="893" height="501" alt="Screenshot 2026-10-15 211539" src="https://github.com/user-attachments/assets/c1af0b4f-580f-4018-b485-0069829c131c" />


### Passenger & Customer Satisfaction Analysis
<img width="893" height="502" alt="Screenshot 2026-10-15 211617" src="https://github.com/user-attachments/assets/0b8b2072-a0ca-4fc6-94d0-9b623afe722b" />


### Aircraft Performance Analysis
<img width="894" height="501" alt="Screenshot 2026-10-15 211640" src="https://github.com/user-attachments/assets/13bf2cad-a266-4661-a1e0-0a5deb31a0f1" />


## Repository Structure

```text
IndiGo-Airlines-Performance-Analysis/
├── README.md
├── IndiGo Airlines — 5-Year Performance Analysis.pbix
└── images/
    ├── overview.png
    ├── load-factor-performance.png
    ├── passenger-customer-analysis.png
    └── aircraft-performance.png
```

## Author

**Partheepan S**  
Aspiring Data Analyst

- **Skills:** Add the tools and skills actually used in this project.
- **GitHub:** https://github.com/aathipartheepan-collab
- **LinkedIn:** www.linkedin.com/in/partheepan-s-305b962ab
