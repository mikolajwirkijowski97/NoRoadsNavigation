# NoRoadsNavigation
A map that tries to make navigating hard terrain a little easier.


# How it will work

## 1. Preprocessing and data collection:
 Gather elevation data. Found this : https://asterweb.jpl.nasa.gov/gdem.asp
 Hydrology data including water flow, swamps etc.
 Terrain classification OR do my own classification.
 Existing roads.
 Plain color data.

## 2. Create a grid of nodes with weights assigned to all edges.
 Assign weights based on terrain type, wetness, slope, amount of trees etc.
 If possible, weight in existing roads.
 Store as an array of uint8 values.
 If needed smooth out the grid values by averaging.


# 3. Run A* algorithm to output connections between points with much lower resolution than the original data.

# 4. Create a local or web app that uses the pre-calculated paths to navigate between 2 points chosen by the user.


