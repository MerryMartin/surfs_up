# surfs_up

## Project Overview
### I want to open a Surf and Shake shop in Hawaii and my potential investor wants to see some weather analysis for the area before he invests.  Specifically, I have prepared a temperature analysis for two different months to ensure that temperature fluctuations won't prevent the surf shop from being viable year-round. 

## Resources
### Analysis was done with the following resources:

* Data Source:
    * hawaii.sqlite

* Software:
   * Python version 3.9.12
   * Jupyter Notebook 6.4.12
   * SQLAlchemy 1.4.39

## Results

* The average temperature in June is 74.94 degrees while the average temperature in December is slightly lower, 71.04 degrees.  
* The minimum temperature recorded, over the years analyzed, was 64.00 degrees for June and 56.00 degrees for December.
* The maximum temperature for June was slightly higher that that of December,  85.00 degrees and 83.00 degrees, respectively. 

![June Summary Stats](https://user-images.githubusercontent.com/115426070/207927353-4d938d18-9b98-4760-881e-546d24c32540.png)


![December Summary Stats](https://user-images.githubusercontent.com/115426070/207927398-ecebd479-f50c-4083-9bf9-5a2ca2594a3e.png)




## Summary

### Temperature Analysis for June and December
* According to the temperature analysis for June and December, the proposed location for the Surf and Shake shop is ideal.  It never gets too cold to want to surf or have ice cream!  

### Additional Analysis
* I would suggest we use another query to study the temperature data for all months of the year, to ensure that the shop could stay open year-round.

   * Example:  annual_results = session.query(Measurement.date, Measurement.tobs).all()







* I would also suggest that we use another query to study the precipitation for the area, to make sure that too much rain wouldn't hurt our new business.

   * Example:  annual_rain_results = session.query(Measurement.date, Measurement.prcp).all()  




