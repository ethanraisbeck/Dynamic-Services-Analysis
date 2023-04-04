# Dynamic-Services-Analysis

## Background

This analysis serves to investigate cycle rates and charge/discharge rates for Dynamic Services for BESS Health optimisation and warranty purposes. Backtests on what a BESS would have been doing should it have participated in these services are carried out on Grid Frequency Data sourced from National Grid at 1s resolution. First we show a distribution of Grid Frequency over 2022 using a random sample of 100k data points to show the levels of deviation from 50Hz.

![Frequency](https://user-images.githubusercontent.com/114344240/229789640-4bb14150-b27f-426d-8656-a935c237409f.png)

Following this, we show response curves from DC, DM and DR to illulstrate how they would respond to these deviations.

![DC](https://user-images.githubusercontent.com/114344240/229790190-17351a2d-5cf5-4a49-91fa-f141837dfa8b.png)
![DM](https://user-images.githubusercontent.com/114344240/229790197-3e45f274-69dc-4c32-8ada-5979708f95a6.png)
![DR](https://user-images.githubusercontent.com/114344240/229790208-0602c5fb-35e2-4b2a-bbb1-86d57ffcc364.png)


## Charge/Discharge Rates

Simulating these reponse curves to the frequency deviations, we can visualise the rate of charge/discharge for each service

![Rate](https://user-images.githubusercontent.com/114344240/229790824-276e66ec-bf51-4b0e-bc23-df630dda34a6.png)

This verifies how aggressive DR is due to the nature of the service and how much more it will cycle the battery and cause higher degredation.

For warranty purposes, the percentage of time spent > 0.8C for DC, DM and DR is 0%, 0.2% and 0.7% respectively.



## Cycle Rates
