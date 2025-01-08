# weather-information-app
The Weather Information App is a Java Swing-based application that provides real-time weather updates for a specified city. It uses the Weatherstack API to fetch current weather information and forecasts. The app includes features such as unit conversion, dynamic backgrounds based on weather conditions, and a search history with timestamps.
Features

Real-Time Weather Updates:

Displays temperature, humidity, wind speed, and weather conditions.

Dynamic backgrounds adjust to the weather condition (e.g., sunny, cloudy, rainy).

Weather Forecast:

Provides a short-term forecast for future dates.

Unit Conversion:

Allows users to switch between Celsius and Fahrenheit for temperature and between km/h and mph for wind speed.

Search History:

Tracks recent weather searches with timestamps.

Error Handling:

Handles invalid city inputs and API errors gracefully.

Requirements

Java Development Kit (JDK) 11 or later.

Internet connection to fetch weather data.

JSON parsing library (org.json).

Setup Instructions

Clone the Repository:

git clone git clone https://github.com/weather-information-app/weather-information-app.git
cd weather-information-app

Add Dependencies:

Download the org.json library from Maven Repository.

Add the JAR file to your project classpath.

API Key:

Replace the API_KEY variable in the code with your Weatherstack API key.

Compile and Run:

Compile the program:

javac -d bin -cp .:json.jar src/com/weather/app/WeatherApp.java

Run the program:

java -cp bin:json.jar com.weather.app.WeatherApp

How to Use

Launch the application.

Enter the name of a city in the text field and click "Get Weather" to view current weather information.

Click "Get Forecast" to see a short-term forecast for the specified city.

Use the "Show in °F" checkbox to switch between Celsius and Fahrenheit.

View your search history at the bottom of the application.

Code Structure

WeatherApp: Main application class.

Handles GUI creation using Swing.

Fetches weather data and updates the display.

API Integration:

Uses HttpURLConnection to fetch data from the Weatherstack API.

Parses responses using the org.json library.

Dynamic Backgrounds:

Changes the background color of the application based on weather conditions.

Known Issues

The free tier of the Weatherstack API does not support future forecasts. Ensure you use a plan that provides this feature if required.

Limited to city-based queries; does not support coordinates or advanced location search.

Future Enhancements

Add support for multiple languages.

Provide hourly weather forecasts.

Include a feature to save search history to a file.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Credits

Developed by Chinwendu Onyeani.

Discussion or Feedback

Feel free to open issues or submit pull requests for improvements. For questions, contact chinwenduonyeani@gmail.com.
