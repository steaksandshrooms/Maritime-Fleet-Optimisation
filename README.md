# Maritime Fleet Optimisation
### 1. Extraction of information from Dataset of 108 bunker ships via SQL
### 2. Mxied-Integer Linear Programming (MILP) programme via PuLP to determine best arrangement of fleet through various metrics within certain constraints.
### 3. Constraints include:
   a. >= 1 ship of every main engine fuel type (LNG, Methanol etc.)
   b. Cumulative Deadweight Tonnage (DWT) or capacity >= ~4.577 million (Average monthly bunker sales volume according to Singapore Maritime POrt Authority (MPA) 2024 Statistics)
   c. Average Safety Rating >=3 (Real World Metric by Rightship)
   d. Each ship can be selected only once
   e. Total journey time <=30 days
4. Various metrics include:
   a. Lowest Cost
   b. Most Environmentally Friendly (least Carbon Intensity Indicator)
   c. Smallest Fleet
   d. Fastest Journey
   e. Highest Safety Rating


   
