# SQLAlchemy Challenge: Surfs Up!

## Project Overview

This project involves using Python, SQLAlchemy ORM, Pandas, and Matplotlib to analyze climate data for Honolulu, Hawaii. The goal is to perform climate analysis, build a Flask API for the data, and assist in planning a vacation to Honolulu.

---

## Features

### Part 1: Climate Analysis and Exploration

1. **Precipitation Analysis**

   - Retrieved the last 12 months of precipitation data.
   - Visualized the data using a line plot.
   - Provided summary statistics of precipitation data.

2. **Station Analysis**
   - Identified the total number of weather stations.
   - Found the most active weather station based on observation counts.
   - Analyzed temperature data for the most active station for the last 12 months.
   - Visualized temperature observations using a histogram.

---

### Part 2: Flask Climate API

Developed a Flask API to expose the analysis results through the following routes:

1. `/`

   - Home page listing all available API routes.

2. `/api/v1.0/precipitation`

   - Returns a JSON dictionary of the last 12 months of precipitation data with dates as keys and precipitation values as values.

3. `/api/v1.0/stations`

   - Returns a JSON list of all weather stations.

4. `/api/v1.0/tobs`

   - Returns a JSON list of temperature observations for the most active station for the last 12 months.

5. `/api/v1.0/<start>` and `/api/v1.0/<start>/<end>`
   - Returns a JSON list of the minimum temperature, average temperature, and maximum temperature for the given date range.
   - If only a start date is provided, the calculations include all dates greater than or equal to the start date.

---

## Data Sources

- `hawaii.sqlite`: SQLite database containing climate data.
- Tables used:
  - `Measurement`: Contains daily weather measurements such as precipitation and temperature.
  - `Station`: Contains weather station information.

---

## Technologies Used

- **Python**: Core programming language.
- **SQLAlchemy**: ORM for database querying and analysis.
- **Pandas**: Data manipulation and analysis.
- **Matplotlib**: Data visualization.
- **Flask**: API development framework.

## License

This project is open source and available under the MIT License.
