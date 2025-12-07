# Mapty

Mapty is a web application designed to help users log and track their running and cycling workouts. By leveraging the browser's Geolocation API and the Leaflet library, the app renders an interactive map where users can drop markers to log specific workout details.

[View the Live Demo](https://novachrono-c-137.github.io/mapty/)

## Table of Contents
1. [About](#about)
2. [Features](#features)
3. [Architecture](#architecture)
4. [Tech Stack](#tech-stack)
5. [Usage](#usage)
6. [Future Enhancements](#future-enhancements)

## About
The main goal of this project is to practice Object-Oriented Programming (OOP) in JavaScript while working with third-party libraries (Leaflet) and browser APIs. It allows users to maintain a persistent log of their physical activities based on location.

## Features
- **Workout Logging:** Users can log both running and cycling workouts.
- **Interactive Map:** Workouts are visualized as markers on a map using the Leaflet library.
- **Geolocation:** The app automatically fetches the user's current coordinates to center the map.
- **Data Persistence:** All workout data is saved to the browser's Local Storage, ensuring data is not lost upon page reload.
- **Form Validation:** Input fields are validated to ensure positive numbers and correct data types.
- **Map Navigation:** Clicking a workout in the sidebar automatically pans the map to the specific workout marker.

## Architecture
The application is built using vanilla JavaScript with a strong focus on Object-Oriented architecture. The structure is divided into the following components:

- **App Class:** The main controller that handles the application lifecycle, including map loading, event listeners, and local storage management.
- **Workout Class:** A parent class containing common data (ID, coordinates, distance, duration, date).
- **Running & Cycling Classes:** Child classes that extend the Workout class to include activity-specific attributes (pace for running, speed for cycling).

## Tech Stack
- **JavaScript (ES6+):** Core application logic.
- **Leaflet API:** Used for rendering maps and managing markers.
- **HTML5 & CSS3:** Layout and styling.
- **LocalStorage API:** For persisting user data.

## Usage
1. **Load the App:** When the application starts, it will request permission to access your location. Accept this to allow the map to center on your position.
2. **Add a Workout:** Click anywhere on the map where you want to log a workout.
3. **Fill Details:** A form will appear in the sidebar. Select the workout type (Running or Cycling) and fill in the distance, duration, and cadence/elevation.
4. **View Logs:** Once submitted, a marker will appear on the map, and the workout details will be listed in the sidebar.
5. **Persist Data:** You can reload the page, and your previous workouts will remain saved.

## Data Management
The application uses the browser's Local Storage to save workout arrays. On initialization, the app checks for existing data and rebuilds the workout objects and map markers accordingly.

## Future Enhancements
The following features are planned for future updates to improve the application:
- Edit and delete functionality for individual workouts.
- Advanced sorting options (by distance, duration, or date).
- Weather API integration to save weather conditions at the time of the workout.
- Detailed workout statistics and charts.
- Functionality to draw lines connecting workout points.
- User authentication and cloud storage sync.
