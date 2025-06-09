# LASALloc – Route Optimization for Air Logistics ✈️

**LASALloc** is a C++ program that simulates an air logistics route planner. It reads airport location data, stores it in a custom linked list, and performs basic geospatial analysis to help determine optimal routing. The program identifies the farthest airport from Austin-Bergstrom International Airport (AUS) and lists all airports within a 100-mile radius of AUS.

## Features

- Custom singly linked list (no STL containers used)
- Stores airport data including name and coordinates
- Calculates distance from AUS using latitude and longitude
- Finds the farthest airport from AUS
- Lists all airports within 100 miles of AUS
- Clean terminal output

## File Structure

## How to Compile and Run

### Requirements
- A C++ compiler (like `g++`)
- Terminal or command line access

### Compilation
```bash
g++ main.cpp Airport.cpp LinkedList.cpp Utilities.cpp -o lasalloc
./lasalloc
Sample Input (airports.txt)
Houston,29.7604,-95.3698
Dallas,32.7767,-96.7970
San Antonio,29.4241,-98.4936
El Paso,31.7619,-106.4850
Austin,30.2672,-97.7431
Sample Output
Farthest airport from AUS: El Paso (Distance: 528 miles)

Airports within 100 miles of AUS:
- San Antonio (Distance: 73 miles)
- Austin (Distance: 0 miles)


