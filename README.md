# Unit 6 - Pythonic Monopoly

![San Francisco Park Reading](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/park-san-francisco.jpg)

## Background

Harold's company has just started a new Real Estate Investment division to provide customers with a broader range of portfolio options. Harold was tasked with building a prototype dashboard and he needs your help. The real estate team wants to trial this initial offering with investment opportunities for the San Francisco market. If the new service is popular, then they can start to expand to other markets.

The goal of this dashboard is to provide charts, maps, and interactive visualizations that help customers explore the data and determine if they want to invest in rental properties in San Francisco.

### Rental Analysis

The first step to building the dashboard is to work out all of the calculations and visualizations in an analysis notebook. Once the code is worked out here, it can be copied over to a dashboard code and used with Panel to create the final layout. Use the `rental_analysis.ipynb` to complete the following:

#### Housing Units Per Year

In this section, you will calculate the number of housing units per year and visualize the results as a bar chart using the Pandas plot function.

Note: By default, the limits auto-scale to the data. However, it is hard to see the difference between the yearly data. In the optional challenge, you can use the min, max, and standard deviation of the data to manually scale the y limits of the plot.

Default Bar Chart

  ![unscaled-bar.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Unscaled%20data.png)

Bar Chart with y-axis limits adjusted

  ![scaled-bar.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Scaled%20data.png)


#### Average Gross Rent in San Francisco Per Year

In this section, you want to visualize the average gross rent per year to better understand the trends for rental income over time. You will visualize the average (mean) gross rent per year and visualize it as a line chart.

1. Calculate the mean `gross` for each year.
2. Visualize the mean gross rent per year as a line chart.

  ![gross-rent.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Avg%20Gross%20rent%20per%20year.png)

#### Average Sales Price Per Year

In this section, you want to determine the average sales price per year to better understand the sales price of the rental property over time. For example, a customer will want to know if they should expect an increase or decrease in the property value over time so they can determine how long to hold the rental property. You will visualize the average (mean) `sales_price_sqr_foot` and visualize it as a bar chart.

1. Calculate the mean `gross` for each year.
2. Visualize the mean gross rent per year as a line chart.

  ![average-sales.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Avg%20sale%20price%20per%20Year.png)

#### Average Prices By Neighborhood

In this section, you want to compare the average prices by neighborhood.

1. Group the data by year and by neighborhood and calculate the average (mean) `sales_price_sqr_foot`.
2. Visualize the mean `sales_price_sqr_foot` per year with the neighborhood as a dropdown selector. Hint: Use hvplot to obtain the interactive dropdown selector for the neighborhood.

  ![avg-price-neighborhood.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Avg%20price%20per%20neighborhood.png)

#### Top 10 Most Expensive Neighborhoods

In this section, you want to figure out which neighborhoods are the most expensive. You will need to calculate the mean sale price for each neighborhood and then sort the values to obtain the top 10 most expensive neighborhoods on average. Plot the results as a bar chart.

  ![top-10-expensive-neighborhoods.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Top%20ten%20most%20expensive%20neighborhood.png)

#### Parallel Coordinates and Parallel Categories Analysis

In this section, you will use plotly express to create parallel coordinates and parallel categories visualizations so that investors can interactively filter and explore various factors related to the sales price of the neighborhoods.

Using the DataFrame of Average values per neighborhood (calculated above), create the following visualizations:

1. Create a Parallel Coordinates Plot

  ![parallel-coordinates.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Parallel%20coordinate%20plot.png)

2. Create a Parallel Categories Plot

  ![parallel-categories.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Parallel%20category.png)
  
 #### Neighborhood Map

In this final section, you will read in neighborhood location data and build an interactive map with the average prices per neighborhood. Use a scatter mapbox object from plotly express to create the visualization. Remember, you will need your mapbox API key for this.

  ![neighborhood-map.png](https://github.com/Tijaw1/Pythonic-Monopoly/blob/main/Sale%20price%20map%20info%20of%20SF.png)


The dashboard is a user interface that shows pertinent informaion regarding San Farancisco area housing and rental history. 

it has four tabs:
Tab 1: is the Welcome tab that has the gross rental information regarding the area and the neighborhoods.
Tab 2: is the yearly market analysis of San Fancisco area.
Tab 3: is the neighborhood analysis page where information regarding the neighborhood and pricing is readily available.
Tab 4: is the parall plot page. this page shows the interactions between various parameters of the housing data.
When the tabs are selected, the dropdown menu provides options as to which type of the data the user is interested in.
