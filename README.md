# 🚲Shared-Bike-Imbalance-Simulation

# 🌐 Overview

This project implements a multi-region shared bicycle system simulation using System Dynamics on the AnyLogic platform. The model abstracts bike flows across three urban regions, tracking the lifecycle of each bike and simulating borrowing and returning behaviors. The simulation explores typical operational scenarios:

🔥 Hotspot Shortage – High-demand regions experiencing rapid bike depletion.

❄️ Coldspot Accumulation – Low-demand regions where bikes accumulate due to low borrowing.

⚖️ Balanced Borrowing and Returning – Supply and demand roughly matched, highlighting time-delay effects.


# ✨ Features

System Dynamics Model: Captures stock-flow relationships between available and in-use bikes.

Scenario Simulation: Adjustable parameters to replicate hotspot shortage, coldspot accumulation, and balanced flow.

Visualization: Time plots of available bikes per region and bikes in use.

Parameter Control: Adjustable variables including arrival rate, return probability, total bikes, and average ride time.


# 🏗️ Model Structure
Stocks

AvailableBikes_A/B/C: Bikes available in regions A, B, and C.

RidingBikes: Bikes currently in use across the system.

Flows

BorrowRate_A/B/C: Bikes borrowed per unit time.

ReturnRate_A/B/C: Bikes returned per unit time.

# 🔄 Key Parameters

ArrivalRate_X: User arrival rate per region.

ReturnProbability_X: Probability that a bike is returned to a given region.

TotalBikes: Total bikes in the system.

AvgRideTime: Average duration of each ride.


# 🛠️ Usage

Open the model in AnyLogic (version X.X or later).

Adjust parameters in the Experiment Setup panel according to the scenario:

🔥 Hotspot Shortage: ArrivalRate_A = 3000, ReturnProbability_A = 0.2

❄️ Coldspot Accumulation: ArrivalRate_C = 200, ReturnProbability_C = 0.4

⚖️ Balanced Flow: similar values for all regions.

Run the simulation and observe TimePlots for AvailableBikes_A/B/C and RidingBikes.

Analyze bike shortages, accumulation, and flow dynamics.


# 📌 Insights from Simulation

🔹 Hotspot regions may face severe shortages without active redistribution.

🔹 Coldspot regions can experience bike accumulation, reducing overall efficiency.

🔹 Even in balanced conditions, return delays can cause temporary shortages.

🔹 Active dispatch, user guidance, or intelligent intervention is necessary for optimal operations.


# ⚠️ Limitations

Only three abstract urban regions are modeled; geographic/environmental factors ignored.

User behaviors simplified as constant arrival and return rates.

No active bike redistribution mechanism; flow relies on natural borrowing/returning behavior.

# 📜 License

This project is released under the MIT License, allowing free use, modification, and distribution for academic and research purposes.
