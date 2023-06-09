# NoRoadsNavigation
A map that tries to make navigating hard terrain a little easier.


# How it will work

1. Preprocessing and data collection:
 1. Gather elevation data. Found this : https://asterweb.jpl.nasa.gov/gdem.asp
 2. Hydrology data including water flow, swamps etc.
 3. Terrain classification OR do my own classification.
 4. Existing roads.
 5. Plain color data.
2. Create a grid of nodes with weights assigned to all edges.
 1. Assign weights based on terrain type, wetness, slope, amount of trees etc.
 2. If possible, weight in existing roads.
 3. Store as an array of uint8 values.
 4. If needed smooth out the grid values by averaging.
3. Run A* algorithm to output connections between points with much lower resolution than the original data.
4. Create a local or web app that uses the pre-calculated paths to navigate between 2 points chosen by the user.


