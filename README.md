# Wildfire Mititgation and Total Cost Prediction

Certain states in the United States such as Colorado and California have experienced enormous losses because of wildfires. The pandemic of wildfires in recent years has resulted in deaths of thousands of people, increases in home-insurance premium and utility bills, and economic downtrends as people move out of areas affected by fires. The causes for wildfires are different. In some places, dangerous fires are wind-driven whereas others are fuel driven. Both federal and state governments spend billions of dollars on managing wildfires with a large portion of this cost being spent on suppression of wildfires.

Research shows that money put towards preparation purposes such as structure hardening of buildings, introducing fuel breaks for community level protection, and creating low intensity prescribed wildfires will reduce the post-wildfire cost impact by six times. Predicting wildfire and total cost will help the government and investors to spend money efficiently in fighting fires and dealing with their potential impacts.

One of the objective of this project is to forecast total cost. 

We extracted data from NIFC[1] and NASF[2] websites. Since the data was recorded by different agencies there wasn't any common key on which we could merge these datasets. Therefore we used a combination of DiscoveryDate, County and State to merge the datasets. 

In the merged data we had some helful features like suppression cost(EstimatedCost), number of structures destroyed, county, state. We were able to collect data for average home costs per county for the years 2017-2019. 

We were able to calculate total damaged structure cost by multiplying the total number of structures destroyed by the average home cost values.

In this notebook we will be loading the merged data, performing some EDA and creating a model to predict total structures destroyed and finally calculate damage cost. 


## References

1. NIFC data <https://data-nifc.opendata.arcgis.com/>
2. NASF data <https://famprod.nwcg.gov/cognos11/bi/?perspective=home>
