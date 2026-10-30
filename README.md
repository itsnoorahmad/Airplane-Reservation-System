# Airplane-Reservation-System
Spring 2026 CS009B Project

A command-line seat reservation program built in Python for UCR's CS009B (Spring 2026). It reads a flight's details from a JSON config file, generates the plane's seat map, and lets a user book and cancel seats from a menu.

## Features
- Loads flight info (flight number, aircraft, origin, destination, date, departure time) from a JSON file
- Generates seats dynamically based on aircraft type (Boeing 717: 10 rows x 5 seats; Airbus A320: 15 rows x 8 seats)
- Displays all seats and their availability
- Books a seat only if it exists and is available
- Cancels a seat only if it belongs to the person requesting the cancellation
- Exports a text itinerary with flight info and seat number

## Concepts Used
- Object-oriented programming (`Seat` and `Airplane` classes, class composition)
- JSON parsing with `json.load()`
- File I/O (reading config, writing itinerary)
- Dictionaries for seat lookup
- Input handling in an interactive CLI menu

## How to Run
1. Keep `airplane_and_reservation_system_python_project.py` and `AirplaneConfigExample.json` in the same folder.
2. Run: `python airplane_and_reservation_system_python_project.py`
3. Choose an option from the menu (1-5).

To change the flight, edit `AirplaneConfigExample.json`. The `aircraft` value must be either `"Boeing 717"` or `"Airbus A320"`.
