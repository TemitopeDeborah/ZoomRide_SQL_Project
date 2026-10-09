# ZoomRide SQL Data Analysis Project

## Project Overview

ZoomRide is a ride-hailing company operating across six African cities. This project uses SQL to analyze trip records and identify revenue trends, customer ride patterns, and vehicle performance.

The goal is to provide actionable insights that help the marketing director make data-driven decisions about city-level marketing campaigns, seasonal demand planning, and vehicle allocation.

## Business Questions

This analysis seeks to answer three key questions:

1. Which city generates the highest revenue?
2. Which month has the highest number of completed rides?
3. Which vehicle type generates the highest revenue?

## Dataset Description

The dataset contains three relational tables:

* **Customers:** Customer information, home cities, signup dates, and signup channels.
* **Drivers:** Driver information, operating cities, vehicle types, ratings, and joining dates.
* **Trips:** Trip dates, cities, distances, fares, trip statuses, and payment methods.

**Data period:** July 2025 – June 2026, based on the trip records.

**Geographic coverage:** Six African cities — Lagos, Abuja, Port Harcourt, Nairobi, Accra, and Kampala.

**Tools used:** MySQL 

## Data Preparation and Cleaning

The dataset contains data quality issues that need to be addressed before reliable reporting.

Key cleaning tasks include:

* Standardizing inconsistent city names, such as `PH` and `Port-Harcourt`, to `Port Harcourt`.
* Correcting spelling variations such as `Nairobbi` and `Kampla`.
* Identifying missing fare values in completed trips.
* Reviewing potential duplicate trip records.
* Excluding cancelled trips from completed-ride and fare-revenue calculations.
  

Cancelled trips have zero fares in the supplied setup data. Missing fares are treated as unknown rather than automatically assumed to be zero.

## Key Findings

### 1. Lagos Generates the Highest Revenue

Lagos is the leading revenue-generating city in the analysis, contributing approximately **₦218,890**, or **38.2% of recorded fare revenue**.

**Business implication:** Lagos represents an important market for customer retention and revenue growth.

**Recommendation:** Prioritize targeted promotions, customer loyalty campaigns, and sufficient driver availability in Lagos while investigating opportunities to improve performance in other cities.

### 2. December 2025 Is the Busiest Month

December 2025 recorded the highest monthly number of completed rides, with **31 completed trips**.

**Business implication:** Higher demand may create opportunities to increase completed rides and revenue during the holiday period.

**Recommendation:** Plan driver availability and seasonal marketing campaigns ahead of December, and compare subsequent years to determine whether this demand peak is recurring.

### 3. Economy Vehicles Generate the Highest Revenue

Economy vehicles generated approximately **₦262,550**, representing **45.8% of recorded fare revenue**. Comfort vehicles generated ₦244,220, while Bikes generated ₦66,870.

**Business implication:** Economy vehicles are the largest recorded revenue contributor, although Comfort vehicles also account for a substantial share.

**Recommendation:** Maintain adequate Economy and Comfort vehicle supply and evaluate revenue per completed trip, operating costs, and profitability before making major fleet-allocation decisions.



## Business Recommendations

Based on the findings, ZoomRide should:

1. **Prioritize Lagos:** Focus customer retention, promotions, and driver supply on its leading revenue market.
2. **Prepare for seasonal demand:** Use December as an initial planning benchmark and validate the pattern with future data.
3. **Optimize vehicle allocation:** Maintain adequate Economy and Comfort supply while assessing profitability by vehicle type.
4. **Improve data quality:** Standardize city names, investigate missing fares, and verify possible duplicate records.


##  Files in This Repository

- [Zoomride Dataset](zoomride_setup.txt)

- [SQL Query Worksheet](zoomride_temitope.sql)

- [Message to the Manager](zoomride_message_to_manager.docx)

- [Answer Sheet](zoomride_answers.txt)

## Conclusion

This project demonstrates how SQL can transform raw ride-hailing data into actionable business insights. The findings identify Lagos as the leading revenue city, December 2025 as the busiest month, and Economy vehicles as the highest revenue-generating vehicle category. The analysis also emphasizes the importance of data quality and industry benchmarks when making marketing and operational decisions.





