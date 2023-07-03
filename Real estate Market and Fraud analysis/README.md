# Researching apartment listings

## Task

From the dataset of archived ads for the sale of apartments in St. Petersburg and nearby area, we need to determine the market value of real estate properties. 

We need to establish the parameters to build an automated system that detects anomalies and fraudulent activity.

For each apartment listing, there are two types of data available. The first type is provided by the user, and the second type is automatically generated based on cartographic data.  


## Data Description

- airports_nearest - distance to the nearest airport in meters (m)
- balcony - number of balconies
- ceiling_height - ceiling height in meters (m)
- cityCenters_nearest - distance to the city center in meters (m)
- days_exposition - number of days the listing was published (from publication to removal)
- first_day_exposition - publication date
- floor - floor number
- floors_total - total number of floors in the building
- is_apartment - apartment (boolean type)
- kitchen_area - kitchen area in square meters (m²)
- last_price - price at the time of removal from publication
- living_area - living area in square meters (m²)
- locality_name - locality name
- open_plan - open floor plan (boolean type)
- parks_around3000 - number of parks within a 3 km radius
- parks_nearest - distance to the nearest park in meters (m)
- ponds_around3000 - number of ponds within a 3 km radius
- ponds_nearest - distance to the nearest pond in meters (m)
- rooms - number of rooms
- studio - studio apartment (boolean type)
- total_area - total area of the apartment in square meters (m²)
- total_images - number of photographs of the apartment in the listing.

## Project perfor plan
Conduct exploratory data analysis and perform instructions:

1) Study the following parameters: area, price, number of rooms, ceiling height. Create histograms for each parameter.
2) Study the time it takes to sell an apartment. Create a histogram. Calculate the mean and median. Describe how long a typical sale usually takes. When can a sale be considered very fast or unusually long?
3) Remove rare and outlier values. Describe any peculiarities you discovered.
4) Check which factors have the greatest impact on the price of an apartment? Investigate whether the price depends on the area, number of rooms, or distance from the city center.
5) Study the dependency of the price on the floor location: first, last, or other. Also, examine the dependence on the listing date: day of the week, month, and year.
6) Select the 10 localities with the highest number of listings. Calculate the average price per square meter in these localities. Identify the localities with the highest and lowest housing prices. This information can be found in the locality_name column.
7) Examine the apartment listings: for each apartment, there is information about the distance to the city center. Select apartments in St. Petersburg (locality_name).
8) Determine which area is considered the city center. Create a column with the distance to the center in kilometers, rounded to whole values.

## Used skills and libraries
*pandas* , *PyMystem3* , *python*, *lemmatization* , *ETL* 

