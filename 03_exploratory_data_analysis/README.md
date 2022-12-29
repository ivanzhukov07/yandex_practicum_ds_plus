# Research of apartments for sale ads

## Description of the project

On the basis of the archive of advertisements for the sale of apartments in St. Petersburg and neighboring cities for several years, you need to learn how to determine the market value of real estate. The first task is to set the parameters. This will allow to build an automated system: it will track anomalies and fraudulent activity. For each apartment for sale, two types of data are available. The first ones are entered by the user, the second ones are obtained automatically on the basis of cartographic data. For example, the distance to the center, airport, nearest park and reservoir.

## Description of data

`airports_nearest` - distance to the nearest airport in meters (m)
`balcony` — number of balconies
`ceiling_height` - ceiling height (m)
`cityCenters_nearest` - distance to the city center (m)
`days_exposition` - how many days the ad was placed (from publication to withdrawal)
`first_day_exposition` - publication date
`floor` - floor
`floors_total` - total floors in the house
`is_apartment` - apartments (boolean)
`kitchen_area` - kitchen area in square meters (m²)
`last_price` - price at the time of unpublishing
`living_area` - living area in square meters (m²)
`locality_name` — name of the locality
`open_plan` - open plan (boolean)
`parks_around3000` - number of parks within a 3 km radius
`parks_nearest` - distance to the nearest park (m)
`ponds_around3000` — number of ponds within a 3 km radius
`ponds_nearest` - distance to the nearest body of water (m)
`rooms` - number of rooms
`studio` - studio apartment (boolean)
`total_area` - area of the apartment in square meters (m²)
`total_images` - the number of photos of the apartment in the ad

## Tools used

`pandas` `numpy` `matplotlib` `math`
