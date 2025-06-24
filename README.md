# URBICA_BOSE_SQL_ASSIGNMENT
SQL_ASSIGNMENT_ON_AIRLINES_DATA


👋 About This Project


This is my first SQL project, where I explored real-world airline operational and revenue data using structured queries.

I focused on developing strong SQL fundamentals by working with multiple interconnected tables, using joins, aggregations, filtering, and window functions.



🛠️ Technologies Used


Database: MySQL

Tool: MySQL Workbench

Language: Structured Query Language (SQL)

🔍 How to Run the Queries



Clone the repository or download the .sql files.

Load the airlines_data schema into your MySQL database (if applicable).

Open MySQL Workbench or your preferred SQL editor.

Copy and run any of the queries provided in the scripts to explore insights.

Each query answers a specific business question and is labeled for clarity.












✈️ Overview of Airlines Data Analysis


We performed a wide-ranging set of analyses on the airlines_data schema to uncover operational, financial, and behavioral insights. The schema included key tables like flights, ticket_flights, tickets, bookings, boarding_passes, aircrafts, and seats.

🔹 Flight-Level Operations


Departure Delays Analysis

Calculated delay in minutes for flights where actual_departure > scheduled_departure.

Focused on flights with a status = 'delayed'.

Flight Usage by Aircraft

Counted total flights and computed average flight duration per aircraft (aircraft_code), joined with aircrafts table.

Occupancy Analysis

Compared number of boarding passes (boarding_passes) to total seats (seats) to calculate occupancy rate per flight.

Frequent Routes Analysis

Counted how many flights operate between each unique departure_airport and arrival_airport pair.

🔹 Revenue and Ticket Analysis


Revenue by Flight

Joined flights and ticket_flights to sum fare amounts and identify top revenue-generating flights.

Revenue by Route

Aggregated total ticket revenue across each unique route (departure_airport to arrival_airport).

Fare Condition Distribution

Counted ticket volume and total revenue across fare types (fare_conditions) like economy, business, etc.

Total Spend per Passenger

Joined tickets and ticket_flights to aggregate how much each passenger_id spent across all bookings.

🔹 Passenger & Boarding Behavior


Passenger Boarding Summary

Counted number of passengers boarding each flight using the boarding_passes table.

Average Boarding Order

Calculated average boarding_no to understand boarding strategy per flight.

🔹 Booking Trends


Daily Booking Trends

Grouped bookings by book_date to analyze volume and total revenue generated per day.

Peak Booking Hours

Extracted hour from book_date and ranked top 5 hours by number of bookings.

🔹 Flight Duration Insights


Average Flight Duration by Aircraft Model

Joined flights with aircrafts to analyze which aircraft models are used for longer or shorter flights.

📊 Tools & SQL Concepts Used


Aggregate Functions: COUNT(), SUM(), AVG(), ROUND()

Date/Time Functions: HOUR(), TIMESTAMPDIFF()

Joins: INNER JOIN, LEFT JOIN

Grouping & Ordering: GROUP BY, ORDER BY, LIMIT

Filtering: WHERE, HAVING, IS NOT NULL

✅ Outcome



This SQL-driven analysis provided insights into:

Flight performance and efficiency

Passenger booking and boarding behavior

Revenue generation by flight, route, and fare type

Operational patterns by airport and aircraft
