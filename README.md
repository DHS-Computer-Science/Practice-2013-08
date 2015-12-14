# Practice 2013 - 08: Excellent Adventure

## Background
You are on a road trip around Virginia with your friends and you only have a
limited amount of gas. There are a series of optional excursions to roadside
attractions. Find the route from your starting city to your destination that
maximizes your units of fun without running out of gas!

Although you may pass through a city multiple times on one road trip, you only
stop and have fun once in each city.

## Description

### Input
The first line of input will be a single integer, c, the number of cities you
can visit. The following c lines will each be a city name followed by a single
space, followed by an integer representing its fun value.

The next line will be a number m, representing the number of roads between
cities that you can travel.

The next m lines each represent one road. Each line includes a city name
followed by a single space and another city name followed by a single space and
the length of the road between the cities in miles (assume all roads are of
integer length). All roads are two directions. The next line is a single integer
p, representing the number of test cases. The following p lines will include the
name of your starting city, a single space, the name of your destination city, a
single space, and the total distance in miles that you are allowed to drive.

City names will include no whitespace (eg. ”VirginiaBeach” is an acceptable
city name, ”Virginia Beach” is not).

### Output
For each case, output the line “Case x:” where x is the case number, on a single
line followed by a space and the optimal path in order. The path should be
expressed as each city that you will drive through in order, space delimited.
Then, on the same line, output the total fun value from the cities that you will
visit. The fun value includes the fun values of your starting and ending cities.

If there is no valid path from the start to destination, instead of a route and
value, print ”Not possible”.

Note that despite any wraparound in the printout, any route is on a single line
with its fun value. If there is any uncertainty in interpretation, consult your
digital copy of the output.

## Sample
### Input
```
10
VirginiaBeach 4
Richmond 5
Charlottesville 10
Blacksburg -5
Roanoke 3
Fredericksburg 3
Danville 8
Harrisonburg 3
Lynchburg 7
Arlington 5
7
VirginiaBeach Richmond 90
Richmond Charlottesville 72
Charlottesville Lynchburg 65
Richmond Fredericksburg 75
Fredericksburg Arlington 40
Lynchburg Roanoke 30
Roanoke Blacksburg 20
3
VirginiaBeach Charlottesville
400
Charlottesville Lynchburg 75
VirginiaBeach Richmond 10
```

### Output
```
Case 1: 29
VirginiaBeach
Richmond
Charlottesville
Lynchburg
Roanoke
Lynchburg
Charlottesville
Case 2: 17
Charlottesville
Lynchburg
Case 3: Not possible
```
