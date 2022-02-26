# surfs_up
Advance data storage and analysis - SQLite, SQLAlchemy, and Flask


## Overview
The purpose of this project was to learn advance data storage and analysis techniques, specifically, by using SQLAlchemy to query SQLite databases, and then to display/transfer the results of those queries to a url (local) by using Flask.  This was done as part of my week 9 project for my DU Data Analytics Bootcamp.  The goals were as follows:
* Explain the structures, interactions, and types of data of a provided dataset
* Differentiate between SQLite and PostgreSQL databases
* Use SQLAlchemy to connect to and query a SQLite database
* Use statistics like minimum, maximum, and average to analyze data
* Design a Flask application using data

To do this, I helped W. Avy, a mock investor, by running data analytics on a weather dataset from the island of Oahu (where he is considering opening a surf shop and icecream store).  I was provided an sqlite file with 5 columns: id, weather station collecting the data, date of datapoint, precepitation score, and temperature observation.  The data consisted of multiple rows of data per day, ranging from the beginning of January 2010 through August 2017.  Once the basic analysis was performed by querying the data in jupyter notebook, I loaded the code into VS Code and developed a Flask application, with 5 routes, to display the data (see Figure 1).  The routes included: Welcome page with a list of available routes; Precipitation scores per date; List of Weather Stations; Monthly Temperature; and Statistics (min temp, average temp, and max temp for given dates).<br><br>
![This is an image](https://github.com/bartblack13/surfs_up/blob/main/Resources/Flask%20code.png)<br><br>
**Figure 1 - Flask code for select routes** <br><br>

## Results: Provide a bulleted list with three major points from the two analysis deliverables. Use images as support where needed.
* Both June and December have similar weather statistics, including average temperatures, 74.9F and 71.0F, respectively (see Figure 2 and 3 below)
* The minimum temperature observation for June was 8 degrees warmer than December (64.0F and 56.0F, respectively), but the maximum temperatures only varied by 2 degrees (85.0F and 83.0F, respectively)
* The standard deviation of June with 1,700 oberservations was 3.257 , where that of December was 3.746, from 1,517 observations

<br><br>![This is an image](https://github.com/bartblack13/surfs_up/blob/main/Resources/June%20Temperature%20Statistics.png)<br><br>
**Figure 2 - June Statistics** <br><br>
![This is an image](
https://github.com/bartblack13/surfs_up/blob/main/Resources/December%20Temperature%20Statistics.png)<br><br>
**Figure 3 - December Statistics** <br><br>


## Summary: Provide a high-level summary of the results and two additional queries that you would perform to gather more weather data for June and December.
In consideration of investing in a surf shop on Oahu that also serves icecream, one could conclude that this is not a bad investment.  Obviously, Hawaii is known for it's surf culture.  The basic statitics, specifically the points mentioned aboce in the Results section, suggest that there is not much difference between June and December temperatures.  As expected, June had a higher miniumum temperature, but only a slightly higher maximum temperature.  The lack of difference in max temp was surprising.  However, the average temperatures for each month only differed by 4 degrees.  The statistics were calculated with similar numbers of data points, although june had a slightly higher sample number, but the standard deviation of each month was very close.  This suggests that the weather variation in December is close to the variation in June.  As expected, June is slightly warmer, but overall, both months would provide ample days to go surfing, and eat icecream. <br><br>
* To provide greater insight into the weather patterns for June and December, one could query the data for each month's precipitation records, and provide similar print outs of precipitaiton statistics.  While rainy weather might not seem ideal to go to the beach in, rainy weather would cause greater swells and larger waves, which would be better for surfing.<br><br>
* Or one could compare the temperatures between the differnt weather stations and determine which area of Oahu might be a better place to open a shop, especially if there is a weather station that collects data very close to the beach, as opposed to inland.  This would give surfers more accurate weather info, if they checked the weather on their phones, for example, as they plan their surf trips.
