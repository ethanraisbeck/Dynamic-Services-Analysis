# Dynamic-Services-Analysis

## Background

This analysis serves to investigate cycle rates and charge/discharge rates for Dynamic Services for BESS Health optimisation and warranty purposes. Backtests on what a BESS would have been doing should it have participated in these services are carried out on Grid Frequency Data sourced from National Grid at 1s resolution. First we show a distribution of Grid Frequency over 2022 using a random sample of 100k data points to show the levels of deviation from 50Hz.

![Frequency](https://user-images.githubusercontent.com/114344240/229789640-4bb14150-b27f-426d-8656-a935c237409f.png)

Following this, we show response curves from DC, DM and DR to illulstrate how they would respond to these deviations.

![DC](https://user-images.githubusercontent.com/114344240/229823572-df5e2d2a-a0ea-40ed-9c7e-43263eed9e37.png)
![DM](https://user-images.githubusercontent.com/114344240/229790197-3e45f274-69dc-4c32-8ada-5979708f95a6.png)
![DR](https://user-images.githubusercontent.com/114344240/229790208-0602c5fb-35e2-4b2a-bbb1-86d57ffcc364.png)

## Charge/Discharge Rates

Simulating these reponse curves to the frequency deviations, we can visualise the rate of charge/discharge for each service

![Rate](https://user-images.githubusercontent.com/114344240/229790824-276e66ec-bf51-4b0e-bc23-df630dda34a6.png)

This verifies how aggressive DR is due to the nature of the service and how much more it will cycle the battery and cause higher degredation.

For warranty purposes, the percentage of time spent > 0.8C for DC, DM and DR is 0%, 0.2% and 0.7% respectively.

## Cycle rates

Now we look at the cycle rates for each service, which will be measured in charges/discharges depending on what service you are in. We can plot a daily average assuming running in each service all day.

![daily](https://user-images.githubusercontent.com/114344240/229818624-71b394e5-72fe-489e-8cf5-aa1c0745b391.png)

Following this we investigate changes in cycling based on a monthly, days in the week and hourly basis.

![monthly](https://user-images.githubusercontent.com/114344240/229820529-41bd3125-0971-4f3c-8c24-92102233baf5.png)


![dayofweek](https://user-images.githubusercontent.com/114344240/229822560-5c0be8f2-c8d4-401f-9f2b-eacf673a59b6.png)


![hour](https://user-images.githubusercontent.com/114344240/229822732-57357034-e7ac-45c0-80fa-09675fc2b2d4.png)

At a monthly level, cycle rates tend to dip around summer time in all services, most likely due to less renewables on the grid meaning increased inertia so more grid stability without use of balancing services. The lowest cycle rate for all services is in August, with the highest tending to be December. The change from lowest to highest is usually a difference between 10-25%.

For the days of the week, 





