# Project Description
Built a robust predictive model that estimates taxi fares for passangers of NYC yellow taxies before their journey begins. Leveraging historical taxi ride data provided by TLC (Taxi & Limousine Commission) of NYC, the model will analyze various factors such as distance, time of day, traffic conditions, and other relevant variables to provide accurate fare predictions. 

Total Attributes:

VendorID                 
tpep_pickup_datetime     
tpep_dropoff_datetime    
passenger_count          
trip_distance            
RatecodeID               
store_and_fwd_flag       
PULocationID             
DOLocationID             
payment_type             
fare_amount              
extra                    
mta_tax                  
tip_amount               
tolls_amount             
improvement_surcharge    
total_amount             

Key Insights from EDA:  
1) The majority of trips were journeys less than 2 miles.
2) Most of the trip costs fall under the range of $5 - $15.
3) Nearly all the tip amounts falls under the $0 - $3 range.
4) Tips amounts are same for each vendor.
5) Nearly two thirds rides were single occupancy.
6) Suprisingly, Wednesday through Saturday had the highest number of daily rides, while Sunday and Monday had the least.
7) Thursday had the highest gross revenue of all days, and Sunday and Monday had the least.

Removed/Imputed outliers trip_distance, fare_amount, duration  
Employeed feature engineering to create new features such as mean_distance, mean_duration, rush_hour, etc.

Model Used: Multiple Linear Regression  
Key Insight: for every 1 mile traveled, the fare increased by a mean of $2.00.
