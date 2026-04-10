# Delhi-Metro-Travel-Analytics
MetroPulse: Delhi Metro Travel Analytics Using Python and SQL

 Project Overview
This project focuses on analyzing metro trip data to uncover insights related to passenger behavior, revenue generation, and travel patterns. The goal is to simulate a real-world data analytics workflow by building a complete pipeline from raw data to actionable insights.

 Objectives
Clean and preprocess raw metro trip data using Python
Store structured data in a SQL database
Perform analytical queries using SQL
Analyze passenger travel behavior
Identify high-demand routes and stations
Evaluate revenue trends and ticket usage

 Tech Stack
Python (Pandas, NumPy) → Data Cleaning
SQL (MySQL) → Data Storage & Analysis
Google Colab / VS Code → Development Environment
Git & GitHub → Version Control

Data Pipeline Architecture
JSON Dataset
     ↓
Python Data Cleaning
     ↓
Cleaned CSV File
     ↓
MySQL Database
     ↓
SQL Analytical Queries
     ↓
Insights & Findings


Data Cleaning Process (Python)

Key preprocessing steps performed:
Loaded JSON dataset into Pandas DataFrame
Removed extra spaces and standardized station names
Handled missing values in ticket types
Converted date column into datetime format
Ensured numeric columns were properly formatted
Removed or handled invalid/missing records

 Database Design (SQL)
A structured table metro_trips was created with the following schema:

TripID (Primary Key)
Date
From_Station
To_Station
Distance_km
Fare
Cost_per_passenger
Passengers
Ticket_Type
Remarks

Indexes were created on frequently queried columns to optimize performance:
Route index (From_Station, To_Station)
Date index
Ticket type index

 SQL Analysis
The dataset was analyzed using SQL queries focusing on:

 *Route Analysis
High passenger traffic routes
Revenue-generating routes
Longest and most frequently used routes

 *Station Analysis
Stations with highest departures
Stations with highest passenger inflow
Most frequently used stations

 *Revenue Analysis
Total revenue generated
Average fare per trip
Revenue contribution by ticket type

 *Passenger Analysis
Average passengers per trip
High-density trips
Passenger distribution by ticket type

 *Travel Pattern Analysis
Peak vs off-peak vs festival trips
Monthly passenger trends
Travel condition impact on revenue

Key Insights
Certain routes consistently show high passenger demand, indicating critical transit corridors
Peak travel conditions contribute significantly to overall revenue
Smart Card usage dominates ticket type distribution
Specific stations act as major hubs with high passenger inflow and outflow
Travel patterns vary significantly across weekdays, weekends, and special conditions
