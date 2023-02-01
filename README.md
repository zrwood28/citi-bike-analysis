# Citi Bike Analysis
Analyzing the usage and trends of Citi Bikes in New York City.

## Analysis
This write up and the accompanying Tableau visualizations are presented with the purpose of analyzing Citi Bike data and trends in New York City. The raw data source can be found here:

https://ride.citibikenyc.com/system-data

### Data Cleaning
Before any analysis was performed, the data had to undergo some cleaning and filtering. The majority of this cleaning can be found in the .ipynb file in this repository. Data was taken from October 2021 up to the most recent month collected, which was September 2022. For the purposes of these analyses, 10,000 items were randomly sampled from each month to create a data pool with 120,000 rides over the past year. Missing values were dropped from this sampling frame and items with ride durations that were over two hours or under one minute were additionally dropped as they were likely instances of misreported information. 

### Tableau Page Link
The Tableau Public page containing the visualizations is linked below:

https://public.tableau.com/views/citibike-analytics/CitiBikeAnalysis?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link

### Members and Casual Riders
The first question that was explored in this analysis was how the breakdown between members and casual riders had functioned over the past year. Within our sampled data, a wide majority of riders were members (Graph 1). There were about three trips by members for every one taken by a casual rider. The only significant movement in this trend was the fact that the proportion was even more member heavy in the winter months, which suggests members are more likely to build Citi Bike usage into their routine, but casual riders may avoid riding in instances of cold weather. With this in mind, it seems that casual riders take longer trips on average (Graph 2). These rides were typically 8 to 9 minutes longer than rides taken by members. Ride duration stays relatively stable for members which may be indicative that frequent users of Citi Bike are using them as transportation or running errands. Casual riders may be more inclined to use a Citi Bike to explore the city or sightsee. Ride duration was more varying for casual users with longer trips in the spring and summer months and shorter ones in January and February.

### Ride Duration by Station
Also displayed are 15 stations with both the shortest and longest trips on average as both starting and ending locations (Graphs 3-6). These visualizations suggest that there is a large disparity in how long people ride for depending on where they depart from and where they are going. For instance, Central Park’s stations are a part of many longer bike rides, likely because some of these rides are taken for leisure rather than efficient travel. Additionally, more popular stations seem to have longer ride times. In the same vein, some stations that are used infrequently proportionally to others are a part of brief journeys; often less than 10 minutes. (Note: Any stations that had less than 10 trips taken within our sampling frame were removed to avoid any fluky data points.)

### Ride Station Popularity on the Map
Manhattan proves to be the most popular location for the use of Citi Bikes, as a vast majority of trips both start and end in this borough (Graph 7). Areas around the Brooklyn Bridge are also commonly used. There seems to be a relatively extreme drop-off anywhere else where the population is less dense and different means of transportation are likely to be more commonplace. Even still, the data used is only a sample of the total ride data, so Citi Bike is extremely popular throughout the city. One significant observation here is that each region does not seem to have a hotspot station; much of the usage is spread evenly in any given neighborhood.
