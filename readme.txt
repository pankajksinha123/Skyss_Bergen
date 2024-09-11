
GTFS Data for Skyss Bergen, Norway (2021-2023)

This repository contains General Transit Feed Specification (GTFS) data for Skyss, the primary public transportation operator in Bergen, Norway. The data spans from November 2021 to October 2023 and provides static information about bus routes, stops, trips, and schedules for the entire Skyss bus network.

Contents:
- GTFS Data: The complete set of GTFS files used for the Skyss bus network in Bergen, Norway.
  - stops.txt: Contains the geographic coordinates and information for all bus stops.
  - trips.txt: Details the sequences of stops for each bus trip, associated with specific routes.
  - stop_times.txt: Lists the scheduled arrival and departure times for each trip at each stop.
  - routes.txt: Defines all the routes operated by Skyss.
  - calendar.txt: Specifies the days of service for each route.
  - shapes.txt: Provides the paths that buses follow on their routes.
  
Data Structure:
The GTFS files describe:
- Stops: Each stop's ID, name, and location (latitude, longitude).
- Trips: Sequences of stops and the routes they belong to.
- Stop Times: Detailed schedules, including arrival and departure times for each stop on each trip.
- Routes: The bus lines, identified by route IDs, and descriptions.
- Shapes: Polylines representing the paths that buses take across the city.

Example:
For example, stop_times.txt aligns each bus stop with scheduled arrival and departure times, providing precise timing for when buses reach each location on their route.

| trip_id | arrival_time | departure_time | stop_id | stop_sequence |
|---------|--------------|----------------|---------|---------------|
| BT001   | 08:45:00     | 08:45:00       | BS123   | 1             |
| BT001   | 08:50:00     | 08:50:00       | BS124   | 2             |
| BT002   | 09:00:00     | 09:00:00       | BS125   | 1             |

Usage:
This GTFS data can be used to analyze bus routes and schedules, develop transit apps, or integrate with demand prediction models for public transportation systems. It provides a foundation for transportation researchers, engineers, and developers to work with real transit data from Bergen.

Reference:
This data adheres to the General Transit Feed Specification (GTFS). For more information on GTFS, visit the official documentation: https://developers.google.com/transit/gtfs/reference.
