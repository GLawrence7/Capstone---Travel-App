# Capstone Project - Travel App

## Table of Contents

* [Overview](#overview)
* [Project Environment Setup](#project)
* [Usage](#usage)
* [UI](#ui)
* [APIs](#api)
* [Tasks](#tasks)

## Overview

Capstone Project - Travel App - This project is web app that obtains a desired trip location & date from the user, and displays weather and an image of the location using information obtained from external APIs. This data is saved to local storage to be displayed when the user returns to the app.

## Usage
City: Enter the city destination
Date: Enter the date of travel
Click Save trip.

This will display the number of days left until the trip, the weather forcast for that date and a picture of the destination if available.

Delete trip button: This will delete the current saved trip and return the user to the initial form.

## Project Environment Setup
Node and Express should be installed on the local machine. The project file server.js should require express(), and should create an instance of their app using express.

The Express app instance should be pointed to the project folder with .html, .css, and .js files.

#### Webpack
Webpack config should contain at least 3 scripts, express server, build and test. Additionally, dev server may be included.

#### Cors
The ‘cors’ package should be installed in the project from the command line, required in the project file server.js, and the instance of the app should be setup to use cors().

#### Body-parser
The body-parser package should be installed and included in the project.

#### Jest
Tests.

#### Service workers
To be implemented at the end of the project. Allows the app to run when the server is not running.

##### Local storage
Persist data so user can return to the site and see their saved trip

## UI
The project will include a simple form where you enter the location you are traveling to and the date you are leaving. The app will save the trip and display a countdown and the weather forcast for location travelling to as well as an image of the location.

#### Input form
A form is present for a user to add trip location and date information

#### Saved trip
Displays the location of the saved trip.

#### Countdown
Displays how many days until the trip.

#### Weather
If the saved trip is within a week, display the current weather forecast
If the saved trip is more than a week away, display predicted forecast.

#### Image
Displays an image of the location the user has saved.

## APIs

#### Geonames API
Returns coordinates for a location.

#### Weatherbit API
Weather API - takes coordinates returned by Geonames Api

#### Pixabay API
Image API - for displaying image of location user will be travelling to

## Dynamic UI

The UI is updated when the user adds or deletes trips, updates the weather and countdown as the trip gets closer.