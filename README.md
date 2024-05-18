# Timestamp Microservice

This is a simple Node.js application that provides an API for converting date strings into Unix timestamps and vice versa. This project is designed to be testable remotely by FreeCodeCamp (FCC) and uses Express.js for handling HTTP requests.

## Features

- Converts date strings into Unix timestamps.
- Converts Unix timestamps into UTC date strings.
- Provides a default date and time (current date and time) if no date is provided.

## Getting Started

### Prerequisites

- Node.js
- npm (Node Package Manager)

## API Endpoints

### GET `/api/:date?`

- **Description:** Returns a JSON object containing the Unix timestamp and UTC date string for the given date input.
- **Parameters:** 
  - `date` (optional): A date string or Unix timestamp. If omitted, the current date and time are used.
- **Response:**
  - If the date is valid:
    ```json
    {
      "unix": 1450137600000,
      "utc": "Fri, 15 Dec 2015 00:00:00 GMT"
    }
    ```
  - If the date is invalid:
    ```json
    {
      "error": "Invalid Date"
    }
    ```



Instructions for building this project can be found at https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/timestamp-microservice
