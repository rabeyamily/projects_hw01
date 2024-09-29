## projects_hw01
# Weather-Based Event Recommender
## Description
This Weather-Based Event Recommender is a Python application that provides event recommendations based on the current weather conditions in a specified city. It combines weather data and upcoming events to offer users a curated list of activities that align with the local climate.

## Features
1. Fetches real-time weather data for any city
2. Retrieves upcoming events in the specified location
3. Recommends events based on current weather conditions
4. Displays event details including name, date, time, and venue (up to 5 events)

## APIs Used

### WeatherStack API

- **Purpose**: Provides current weather information for a specified city.
- **Why Chosen**: WeatherStack offers a straightforward API with reliable data and easy integration for fetching real-time weather conditions.

### Ticketmaster API

- **Purpose**: Retrieves event listings based on location and date range.
- **Why Chosen**: Ticketmaster is a well-known platform for event discovery, making it a suitable choice for finding a variety of local events.

## Prerequisites
Before running this application, we must obtain API keys for WeatherStack and Ticketmaster.
1. WeatherStack API key: Get it here: https://weatherstack.com/
2. Ticketmaster API key: Get it here: https://developer.ticketmaster.com/

## Usage
1. Run this: python weather_event_recommender.py
2. When prompted, enter the name of a city.
3. The application will display the current weather and a list of recommended events for the next 7 days.

## Example Output

## Error Handling
1. Invalid city names
2. API request failures
3. Timeout errors
If an error occurs, the user will be prompted to try again with a different city name.

## Rate Limiting
This application respects the rate limits of both APIs. It implements a timeout of 10 seconds for each API request to prevent hanging in case of slow responses.
