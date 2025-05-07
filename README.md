# Module 6 Challenge: Python API Analysis 

## Overview

The Module 6 Challenge involved building two Python-based applications that use APIs to analyze weather data and suggest vacation destinations:

1. **WeatherPy** – Created a dataset of weather conditions across hundreds of cities worldwide using the OpenWeatherMap API and visualized the results.
2. **VacationPy** – Used the weather data to identify ideal vacation spots and plotted nearby hotels using the Geoapify API.

---

## Technologies Used

- Python 3
- Jupyter Notebook
- pandas
- matplotlib
- citipy
- requests
- OpenWeatherMap API
- Geoapify API
- JSON
- gmaps (for map visualizations)
- dotenv (for secure API key usage)

---

## Part 1: WeatherPy

### Process

- Generated random latitude and longitude pairs.
- Used `citipy` to find the nearest city for each coordinate.
- Fetched weather data for each city using the OpenWeatherMap API.
- Saved the data into a CSV file.
- Created scatter plots to show the relationships between:
  - Latitude vs. Temperature
  - Latitude vs. Humidity
  - Latitude vs. Cloudiness
  - Latitude vs. Wind Speed
- Performed linear regression on the above relationships for both the Northern and Southern hemispheres.

### Outputs

- A CSV file containing weather data for 500+ cities.
- Visualizations saved as PNG files for each scatter plot and linear regression.

---

## Part 2: VacationPy

### Process

- Filtered cities from the WeatherPy dataset to find ideal vacation conditions (e.g., low wind, comfortable temperature, low humidity).
- Used Geoapify API to locate the nearest hotel for each selected city.
- Mapped vacation spots using `gmaps`, showing:
  - Hotel name
  - City and country
  - Weather conditions

### Outputs

- CSV file with filtered vacation cities and hotel info.
- A heat map and hotel marker map saved as images.

---

## Results Summary

- WeatherPy demonstrated clear relationships between weather metrics and latitude.
- VacationPy effectively used multiple APIs to recommend real-world travel locations based on weather preferences and nearby hotels.

---

## Author

Manuel Guevara – Data Analytics Bootcamp Student

## License

This project is for educational purposes only.
