# surfs_up

## Project Overview
### I want to open a Surf and Shake shop in Hawaii and my potential investor wants to see some weather analysis for the area before he invests.  Specifically, I have prepared a temperature analysis for two different months to ensure that temperature fluctuations wouldn't prevent the surf shop would be viable year-round. 

## Resources
### Analysis was done with the following resources:

* Data Source:
** hawaii.sqlite

* Software:
** Python version 3.9.12
** Jupyter Notebook 6.4.12
** SQLAlchemy 1.4.39

## Results
Provide a bulleted list with three major points from the two analysis deliverables. Use images as support where needed.  There is a bulleted list that addresses the three key differences in weather between June and December. (6 pt)
* The average temperature in June is 74.94 degrees while the average temperature in December is slightly lower, 71.04 degrees.  
* The minimum temperature over the years analyzed was 64.00 degrees for June and 56.00 degrees for December.
* The maximum temperature for June was slightly higher that that of December,  85.00 degreen and 83.00 degrees, respectively. 

(insert June image)

(insert December image)





## Summary

### Temperature Analysis for June and December
* According to the temperature analysis for June and December, the proposed location for the Surf and Shake shop is ideal.  It never gets too cold to want to surf or have ice cream!  

### Additional Analysis
* I would suggest we use another query to study the temperature data for all months of the year, to ensure that the shop could stay open year-round.

** annual_results = session.query(Measurement.date, Measurement.tobs).all()


(insert image of annual results)



* I would also suggest that we use another query to study the precipitation for the area, to make sure that too much rain wouldn't hurt our new business.

** annual_rain_results = session.query(Measurement.date, Measurement.prcp).all()  


(insert image of annual rain results)
