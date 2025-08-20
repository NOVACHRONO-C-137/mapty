# Mapty App Documentation 🗺️

## 📑 Table of Contents
1. [Introduction](#introduction)
2. [✨ Features](#features)
3. [🏗️ Architecture](#architecture)
4. [🎨 User Interface](#user-interface)
5. [⚙️ Core Functionality](#core-functionality)
6. [💾 Data Management](#data-management)
7. [🗺️ Map Integration](#map-integration)
8. [🎭 Styling](#styling)
9. [🚀 Future Enhancements](#future-enhancements)

## 🔎 Introduction
**Mapty** is a web application that allows users to log and track their workouts on an interactive map. Users can add running or cycling workouts, view their workout history, and see their workout locations on a map.

👉 [LIVE DEMO OF THE APP](https://novachrono-c-137.github.io/mapty/)  


## ✨ Features
- 🏃 Log running and cycling workouts  
- 🗺️ Display workouts on an interactive map  
- 💾 Store workout data locally  
- 📋 View a list of all workouts  
- 📍 Automatically detect user's location  

## 🏗️ Architecture
The app is built using **vanilla JavaScript** with an **object-oriented approach**. It consists of the following main components:

1. `App` class: The main application controller  
2. `Workout` class: Base class for workouts  
3. `Running` and `Cycling` classes: Specific workout types  
4. **Leaflet library**: For map functionality  

## 🎨 User Interface
The UI is divided into two main sections:  
1. **Sidebar** 🗂️: Contains the form for adding new workouts and the list of saved workouts  
2. **Map** 🗺️: Displays the interactive map with workout markers  

## ⚙️ Core Functionality

### 📍 Geolocation
- Uses the **browser's geolocation API** to get the user's current position  
- Shows an alert if geolocation is not available  

### ➕ Adding Workouts
1. User clicks on the map to set the workout location  
2. A form appears for entering workout details  
3. User selects the workout type (running or cycling) and enters details  
4. On form submission, a new workout is created and added to the list and map  

### 🖼️ Displaying Workouts
- Workouts are displayed in a **list** in the sidebar  
- Each workout is represented by a **marker** on the map  
- Clicking on a workout in the list centers the map on that workout's location  

## 💾 Data Management
- Workouts are stored in the **browser's local storage**  
- Data persists across page reloads  
- A reset function is available to clear all stored data  

## 🗺️ Map Integration
- Uses the **Leaflet library** for map functionality  
- Custom markers and popups display workouts on the map  

## 🎭 Styling
- Uses a custom **CSS file** for styling  
- CSS variables ensure consistent color theming  
- Layout is **responsive** with Flexbox and Grid  

## 🚀 Future Enhancements
Potential areas for improvement and new features:  
1. ✏️ Ability to edit and delete workouts  
2. 📊 More detailed workout statistics  
3. 🌦️ Weather data integration for workout locations  
4. 🔀 Ability to sort workouts by different criteria  
5. 📤 Export workouts (GPX, CSV, etc.)  
6. 👤 User accounts and cloud sync
