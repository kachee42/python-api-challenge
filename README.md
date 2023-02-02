# python-api-challenge

## Weather Analysis

The purpose of this code was to generate a large list of cities all around the world and analyze the weather data in those cities. The maximum temperature, humidity, wind speed, and cloudiness were all evaluated in each of at least 500 cities. Note that the code to determine the cities was randomly generated and therefore the cities selected and the number of those cities will vary each time the code is executed. Below is a small sampling of what the city data looked like when the code was executed Feb 1, 2023 at around 6:00PM PST.

![image](https://user-images.githubusercontent.com/118322354/216241892-d6211fb5-6898-4218-b882-d7d42b57dab7.png)

Each of these variables was plotted in a scatter plot against latitude. The scatter plots as generated on Feb 1, 2023 at around 6:00PM PST are below.

![image](https://user-images.githubusercontent.com/118322354/216245933-c18d518f-4df2-43f9-bc40-b58f5a701de4.png)

[image](https://user-images.githubusercontent.com/118322354/216246105-244dbb6d-9500-43f8-8926-f5c079e7d34b.png)

![image](https://user-images.githubusercontent.com/118322354/216246210-1160b572-3492-47b8-9bff-a51e9fc3a969.png)

The data was then seprated into northern and southern hemispheres and the plots were done again for each hemisphere. Regressions and pearson r values were calculated to determine the correlation between latitude data and the weather variable data for each hemisphere. Plots, r values, and interpretation for each plot are below. The table of Pearson r-values and correlation strength used is at the bottom of the 8 plots.

![image](https://user-images.githubusercontent.com/118322354/216246648-c45b7055-e0f1-4b6b-9ba4-7df5ad93454b.png)

In the northern hemisphere there is a very strong correlation between maximum temperature and latitude.

![image](https://user-images.githubusercontent.com/118322354/216246732-9a195447-8123-4c6a-a665-3c45158ddcfb.png)

In the southern hemisphere there is a weak correlation between maximum temperature and latitude

![image](https://user-images.githubusercontent.com/118322354/216247247-2aa082bb-23e0-4c05-b848-eb7a49798a24.png)

In the northern hemisphere there is a moderate correlation between humidity and latitude.

![image](https://user-images.githubusercontent.com/118322354/216247350-5bd14937-e731-411a-9aaf-bd27a6c8c6e3.png)

In the southern hemisphere there is a weak correlation between humidity and latitude.

![image](https://user-images.githubusercontent.com/118322354/216247989-995e4599-c691-4a84-b4d3-3fcc5876c2d6.png)

In the northern hemisphere there is a weak correlation between cloudiness and latitude.

![image](https://user-images.githubusercontent.com/118322354/216248076-dba51c1d-162c-47d0-a8d0-e870affa3e6d.png)

In the southern hemisphere there is a weak correlation between cloudiness and latitude.

![image](https://user-images.githubusercontent.com/118322354/216248294-fffe8d36-f10d-4698-9229-5742a4c3a499.png)

In the northern hemisphere there is no correlation between wind speed and latitude

![image](https://user-images.githubusercontent.com/118322354/216248339-4c2692ac-f86b-4f1d-8124-cc345324e39d.png)

In the southern hemisphere there is a weak correlation between wind speed and latitude

![image](https://user-images.githubusercontent.com/118322354/216248790-b6fc0151-9a7d-4fd6-9fbb-18fe7d711746.png)

Please note that while these calculations hold true at the time that the code was run, the correlations may be stronger or weaker than evaluated here when the code is executed at a different date or another time of day.

## Vacation Spot Analysis

Using the locations and weather data gathered in the weather analysis the cities were plotted on a world map, with dot size determined by the humidity at that location. The map of the locations and humidities as found when the code was executed on Feb 1, 2023 is below.

![image](https://user-images.githubusercontent.com/118322354/216251294-7589988f-2f4f-46da-aee7-8e95662a6d46.png)

Personal ideal weather conditions were used to narrow down the list of cities. The conditions sought were a max temperature between 18C and 26C, humidity between 10% and 20%, cloudiness less than or equal to 50% and wind speed of less than 5 m/s. The cities that met these conditions at the time of code execution can be seen in the table below.

![image](https://user-images.githubusercontent.com/118322354/216251844-1177f29b-bc6a-4296-97bd-640d2500ab8e.png)

A search was executed through geoapify to find the nearest hotel to the coordinates of the city and were added to a new table as follows. Please note that when this code was executed several of the randomly selected cities that met the weather criteria were remote cities that did not have a hotel within 10km of the center of the city. When the code is executed at another point in time it is likely there there may be more or fewer cities and those cities may or may not have hotels within the specified 10km of the city center.

![image](https://user-images.githubusercontent.com/118322354/216252575-663e3958-3575-40c1-befa-869f8355fe1d.png)

The cities matching the "ideal" weather conditions were then plotted on a world map. At the time of execution the cities were near the equator in several different African countries as well as one in India and one in Thailand. The plot can be seen below.

![image](https://user-images.githubusercontent.com/118322354/216252968-0c7f8f49-2a28-485d-82d9-71b39b15e146.png)
