# Maritime Fleet Optimisation
#### 1. Extraction of information from Dataset of 108 bunker ships via SQL
Dataset Includes:
• Vessel	ID, name, vessel type	
• AIS	vessel movement data	–
- date/time	stamp, latitude/longitude positions	
- Positional information - at	anchor, in port	
• Cargo carrying capacity (DWT in tonnes)	
• Design	speed	(Vref)
• Machinery	powers/load	
• Main Engine (P)
• Auxiliary	engine (ael)	
• Auxiliary	Boiler (abl)	
• Fuel type	—	
- Fuel type the ship	is	designed	to	burn in	its above	three	machineries	
§ main_engine_fuel_type	
§ aux_engine_fuel_type	
§ aux_boiler_fuel_type	
o Specific	fuel	oil	consumption	(sfc)	for	each	of	the	above	three	
machineries	
§ sfc_me	
§ sfc_ae	
§ sfc_ab	
• Ship	Safety	Score	—	integer	1–5	(1=	Highest	Risk;	5	=	Least	Risk)	
#### 2. Mixed-Integer Linear Programming (MILP) programme via PuLP to determine best arrangement of fleet through various metrics within certain constraints.
#### 3. Constraints include:
##### a. >= 1 ship of every main engine fuel type (LNG, Methanol etc.)
##### b. Cumulative Deadweight Tonnage (DWT) or capacity >= ~4.577 million (Average monthly bunker sales volume according to Singapore Maritime POrt Authority (MPA) 2024 Statistics)
##### c. Average Safety Rating >=3 (Real World Metric by Rightship)
##### d. Each ship can be selected only once
##### e. Total journey time <=30 days
#### 4. Various metrics include:
##### a. Lowest Cost
##### b. Most Environmentally Friendly (least Carbon Intensity Indicator)
##### c. Smallest Fleet
##### d. Fastest Journey
##### e. Highest Safety Rating


   
