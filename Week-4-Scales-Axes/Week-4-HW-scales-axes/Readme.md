This week we learned about scales, axes, and loading data.

# Scales
- Necessary so D3 can scale the data to fit within the screen size
- Can be used to add a color scale, with ah range of colors

## Different scales
1. **d3.scaleLinear()**
   1. Most common scale - maps continuous quantitative data
   2. Normalizes the data
   3. Can either manually set the min/max or use d3.min & d3.max, which automatically set the min/max values to the min/max values in the data
2. **d3.scaleBand()**
   1. Maps discrete values in order and evenly spaced out
   2. No max/min b/c it is ordinal data (non-numeric)
   3. Domain is usually a data.map and the specified column
   

## Domain and Ranges
- Domain (input) = data
- Range (output) = visual
- *D3 must take a large dataset and scale it down to the appropriate screen size*

# Axes
- Use the axes and ticks to measure data on graphs 
- Append to SVG using ("g") - g = group
- *Must always use .call() to call the axes or else it won't display on DOM*
  
  **4 types**
1. d3.axisTop
2. d3.axisBottom (common)
3. d3.axisLeft (common)
4. d3.axisRight

# Loading data
- d3 can accept different types of data (ex; json)
- Use d3.csv to load data as a promise so it doesn't have to wait
- Then give the dataset a variable name
- Console log the data to ensure it loaded properly
- Format if needed


# Homework
- Create a simple dataset and either construct a bar chart or scatter plot based on the data
- Style and format
- Try to add a title to chart


## Dataset
I compiled a dataset of my poor sleep habits. My sleep has deteriorated since the start of the pandemic and has only worsened. I tracked days, hours slept, and quality rating. I then visualized the data as a scatter plot. 

![picture of scatterplot of sleep data](sleep_data.jpg)  


## What worked and what didn't for the hw
- Was able to load the data, create a chart, and create the axis
- Was able to move the SVG over a bit so the left axis wasn't smushed against the left side of the screen
- Was able to add a chart title
- Was able to create both a bar and scatter plot - little hard to decide which is better. Opted for scatter because it display the data more than the bar. 
- Shifted the axes up and to the right because they were too close to the margins, so the axes labels would disappear when you added some spacing
- Had to reorder the csv file manually in order for the x-axis to order properly


- Unable to add all data labels - it only shows some


## Remember for the future
D3 pulls the unique values in the order in which they appear in the dataset and maps them to the x-axis.


 