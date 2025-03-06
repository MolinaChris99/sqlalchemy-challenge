### SQLAlchemy Challenge Overview ### 
In this project, students were tasked with acting as a traveler preparing to visit Hawaii. The goal was to analyze climate data for Hawaii and build a Flask API to serve the results. The dataset provided included historical weather information such as temperature and precipitation, collected from various weather stations across the island.

* Part 1: Climate Data Analysis

- The SQLite database was connected using SQLAlchemy.
- The schema for the database, which includes both the measurement and station tables, was mapped.
- The most recent 12 months of precipitation data were queried and loaded into a Pandas DataFrame, sorted by date.
- A time-series graph of the precipitation data was generated.
- Summary statistics for the precipitation data were calculated.
- The total number of weather stations was determined, and the most active station (based on the number of observations) was identified.
- The temperatures for the most active station were queried for the last 12 months and visualized using a histogram.

* Part 2: Flask API Development

- /(Homepage): Displays a list of all available API routes.
- /api/v1.0/precipitation: Provides the last 12 months of precipitation data as a JSON dictionary, with dates as keys and precipitation values as the corresponding values.
- /api/v1.0/stations: Returns a JSON list of all weather stations included in the dataset.
- /api/v1.0/tobs: Returns a JSON list of temperature observations for the most active station from the past 12 months.
- /api/v1.0/<start_date>: Accepts a start date (in YYYY-MM-DD format) and returns a JSON object with the minimum, average, and maximum temperatures for all dates on or after the given start date.
- /api/v1.0/<start_date>/<end_date>: Accepts a start and end date (in YYYY-MM-DD format) and returns a JSON object with the minimum, average, and maximum temperatures for the dates between the start and end date.

* Resources Used:

1) Class lectures and recorded sessions
2) YouTube tutorials
3) Assigned group work
4) ChatGPT assistance
