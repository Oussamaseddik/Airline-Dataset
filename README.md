Airline Dataset Analysis - Power BI Dashboard ✈️📊

📢 Project Overview

This project presents an interactive Power BI dashboard analyzing airline performance using real-world data. The dashboard provides insights into flight patterns, delays, passenger trends, and airline performance across different regions and time periods.

📊 Key Features & Visuals

🛫 Flight Trends Over Time → Line chart displaying daily/monthly flight data.

⏳ On-Time Performance & Delays → Bar charts comparing on-time flights vs. delayed flights.

📍 Geographic Flight Analysis → Map visualization showing flight routes and passenger density.

📅 Seasonal Trends → Identify peak and off-peak seasons for airline traffic.

🚀 Top Performing Airlines → Ranking airlines based on passenger volume and delay rates.

📈 Passenger Growth Analysis → Percentage change in passengers over months/years.

📌 DAX Measures Used

Total Flights → SUM(AirlineData[Flight_Count])

Average Delay Time → AVERAGE(AirlineData[Delay_Minutes])

On-Time Performance Percentage → DIVIDE( COUNTROWS(FILTER(AirlineData, AirlineData[Delay_Minutes] = 0)), COUNTROWS(AirlineData) ) * 100

Passenger Growth Rate → DIVIDE( SUM(AirlineData[Passengers]) - SUM(AirlineData[Previous_Passengers]), SUM(AirlineData[Previous_Passengers]) ) * 100

Top Airline by Passenger Volume → TOPN(1, SUMMARIZE(AirlineData, AirlineData[Airline], "Passengers", SUM(AirlineData[Passengers])), [Passengers], DESC)

📂 Dataset Overview

Flight_Date → Date of flight.

Airline → Airline name.

Flight_Count → Number of flights per record.

Delay_Minutes → Delay duration per flight.

Passengers → Total number of passengers per flight.

Origin & Destination → Airport codes for flight routes.

Flight_Status → On-time, delayed, or canceled.

Weather_Impact → Influence of weather on flights.

🔧 How to Use the Dashboard

Load the dataset into Power BI.

Use provided DAX measures to generate insights.

Apply filters (year, airline, flight status) for deeper analysis.

Analyze visualized trends to explore flight performance.

🚀 Future Enhancements

Predictive modeling for flight delays based on historical data.

Integration with real-time flight tracking APIs.

Customer satisfaction analysis based on airline performance.

📌 Tools & Technologies Used

Power BI → Data visualization & reporting.

DAX (Data Analysis Expressions) → Custom calculations.

Excel/Python (Pandas) → Data preprocessing & transformation.

📬 Contact & Contribution

Feel free to fork this repository, suggest improvements, or contribute additional features! If you have any questions or ideas, reach out via linkedin : www.linkedin.com/in/oussama--seddik

