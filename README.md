# British Airways Reviews Dashboard

## Overview

This project is an interactive Tableau dashboard built from British Airways review data. It explores customer experience across countries, months, aircraft types, traveler segments, and seat classes. The dashboard is designed as an end-to-end portfolio project that demonstrates data preparation, parameter-driven analysis, calculated fields, visual design, and dashboard interactivity.

The main goal of the project is to let users dynamically switch between key review metrics and investigate how ratings vary across geography, time, and aircraft categories.

## Project Features

* Interactive metric selector using a Tableau parameter
* Dynamic calculated field that updates visuals based on the chosen metric
* Country-level filled map for geographic analysis
* Monthly trend line chart
* Aircraft comparison chart with both average rating and review volume
* Summary KPI section for core service dimensions
* Dashboard-wide filters for:

  * Review month
  * Seat type
  * Traveler type
  * Aircraft group
  * Continent
* Visuals configured to act as filters for cross-highlighting and drill-down exploration

## Metrics Included

Users can switch between the following metrics:

* Overall Rating
* Cabin Staff Service
* Entertainment
* Food & Beverages
* Ground Service
* Seat Comfort
* Value for Money

## Dataset

The project uses two CSV files:

### 1. `ba_reviews.csv`

Contains individual British Airways reviews, including:

* Author
* Date
* Country / place
* Aircraft
* Traveler type
* Seat type
* Ratings across multiple service categories

### 2. `countries.csv`

A country mapping table used to enrich the review data with geographic grouping fields such as continent and region.

## Data Model

The Tableau data model uses a relationship between the two tables:

* `ba_reviews.place`
* `countries.country`

This relationship enables the use of geographic filters such as continent while preserving the original review-level data.

## Dashboard Views

### 1. Average Metric by Country

A map showing the average selected metric by country.

### 2. Average Metric by Month

A line chart that displays how the selected metric changes over time.

### 3. Average Metric by Aircraft

A comparison chart showing:

* Average selected metric by aircraft group
* Number of reviews by aircraft group

### 4. Summary KPI Panel

A compact overview of the average values for the major service categories.

## Key Tableau Techniques Used

* Parameters
* Calculated fields
* Geographic roles
* Relationships between tables
* Custom tooltips
* Filter actions
* Formatting and dashboard layout design
* Grouping low-frequency aircraft into a `Various` category

## Interactivity

The dashboard is built to be highly interactive:

* Selecting a metric updates all relevant visualizations
* Filters apply across the dashboard
* Clicking on a month, country, or aircraft filters the other charts
* Tooltips provide both average score and review count context

## Project Workflow

1. Connect both CSV files in Tableau
2. Define the relationship between review data and country mapping data
3. Assign geographic role to the country field
4. Create a parameter for metric selection
5. Build a calculated field to return the selected metric
6. Create dashboard filters
7. Group aircraft with low review counts into a single category
8. Build the map, trend chart, aircraft chart, and KPI section
9. Assemble the final dashboard using floating elements and layout formatting
10. Publish to Tableau Public


## Tools Used

* Tableau Public / Tableau Desktop
* CSV data files



## Portfolio Value

This project is a strong portfolio piece because it demonstrates:

* End-to-end dashboard development
* Data cleaning and modeling decisions
* User-focused interactivity
* Clean dashboard design
* Analytical storytelling through visual exploration




## Tableau Public Link

(https://public.tableau.com/app/profile/dan.mark.rivera.tolod/viz/BritishAirwaysReview_17730236205550/Dashboard1)
```


