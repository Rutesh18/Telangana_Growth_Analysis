# Analyse Growth and Present Insights to the Telangana Government
As part of the codebasics resume project challenge 7, I have worked on this analysis project.

Link to the [challenge](https://codebasics.io/challenge/codebasics-resume-project-challenge)

Link to [Interactive Dashboard](https://www.novypro.com/project/analyse-growth-and-present-insights-to-the-telangana-government)

Link to Project Presentation

# Task 
To Analyse the data set and present growth insights to the Telangana Government

Telangana is one of the fastest-growing states in India and one of the states with an open data policy. (They have published all their data online). 
The task is to analyse Telangana’s growth among different sectors quantitatively and provide useful Insights to the Telangana government that would help them to make data-informed decisions that would further support the growth of the state.
I have build a Power BI dashboard and did some analysis using SQL

# Explore Data set
This file contains all the meta information regarding the columns described in the CSV files. We have provided 5 CSV files:
1. dim_districts
2. dim_date
3. fact_stamps
4. fact_transport
5. fact_TS_iPASS

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Column description for dim_districts:
The table contains information about districts.

- dist_code: This column represents the district code or identifier for each district.

- district: This column represents the name of the district.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Column description for dim_date:
This table contains the dates at the monthly level. Please be aware that the fiscal year of Telangana spans from April to March.

- month: This column contains the starting date of each month.

- Mmm: This column contains the name of the month.

- quarter: This column contains the associated quarter for each particular month.  

- fiscal_year: This column contains the corresponding fiscal year of each month.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Column description for fact_stamps:
The table provides data on the revenue generated from document registrations and estamp challan payments aggregated at the district and monthly level.

- dist_code: This column represents the district code.

- month: This column represents the starting date of each month.

- documents_registered_cnt: This column represents the total count of documents registered.

- documents_registered_rev: This column represents the total revenue generated from the registered documents.

- estamps_challans_cnt: This column represents the count of e-stamps challans.

- estamps_challans_rev: This column represents the revenue generated from e-stamps challans.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Column description for fact_transport:
The table provides information about the individual vehicle sales data from the RTA(Regional Transport Authority) of the state of Telangana categorized by fuel type,
vehicle class, seating capacity, and other general categories aggregated at the district and monthly level.

- dist_code: This column represents the district code.

- month: This column represents the starting date of each month.

- Vehicle sales categorized by different fuel types:
	fuel_type_petrol: Number of vehicles sold with petrol fuel type.
	fuel_type_diesel: Number of vehicles sold with diesel fuel type.
	fuel_type_electric: Number of vehicles sold with electric fuel type.
	fuel_type_others: Number of vehicles sold with other fuel types.

- Vehicle sales categorized by different vehicle class:
	vehicleClass_Motorcycles: This category includes all two-wheeled vehicles, such as motorcycles, scooters etc.
	vehicleClass_Motorcars: This category includes all four-wheeled vehicles, such as cars, vans etc.
	vehicleClass_Auto rickshaws: This category includes three-wheeled vehicles, such as auto rickshaws.
	vehicleClass_Agriculture: This category includes all vehicles used for agricultural purposes, such as tractors and harvesters.
	vehicleClass_Others: This category includes all vehicles belonging to other classes.

- Vehicle sales categorized by seating capacity
	seatCapacity_1_to_3: Number of vehicles sold with a seating capacity ranging from 1 to 3.
	seatCapacity_4_to_6: Number of vehicles sold with a seating capacity ranging from 4 to 6.
	seatCapacity_above_6: Number of vehicles sold with a seating capacity above 6.

- Sales of vehicles by other categories:
	Brand_new_vehicles: Number of brand new vehicles sold.
	Pre-owned_vehicles: Number of pre-owned vehicles sold.
	category_Non-Transport: Number of vehicles in the non-transport category sold. The Non-Transport category typically includes vehicles that are not primarily used for public transportation of passengers or goods. Instead, these vehicles are generally intended for personal use, recreational activities, agriculture, construction, and other non-commercial purposes.
	category_Transport: Number of vehicles in the transport category sold. The Transport category comprises vehicles primarily designed and used for the transportation of goods, passengers, or both. These vehicles are generally associated with commercial and public transportation purposes.

---------------------------------------------------------------------------------------------
# Column description for fact_TS_iPASS:
The TS-iPASS dataset in Telangana comprises data concerning units or businesses established within the state under the "Industrial Project Approval and Self-Certification System" (iPASS). This government initiative aims to foster industrial growth and investment by streamlining project approvals and enabling self-certification for businesses.
For further details, visit: https://ipass.telangana.gov.in/


- dist_code: This column represents the district code.

- month: This column represents the starting date of each month.

- sector: This column represents the industry category. Examples of sectors include 'Automobiles', 'Beverages', 'Engineering', 'Food Processing', etc.

- investment in cr: The column represents the investment made in the specific sector, measured in crores (a unit of currency), for the corresponding district and month.

- number_of_employes: This column represents the number of employees associated with that sector for given district and respective month.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Data Modelling 
![Data Modelling](https://github.com/Rutesh18/Telangana_Growth_Analysis/assets/115866652/5934b00b-0c67-4cc2-8b1e-da9424e723b9)


# Stamp Overview 
![Stamp Overview](https://github.com/Rutesh18/Telangana_Growth_Analysis/assets/115866652/32506730-02f6-4a82-befc-0c53b37020a4)


# Transport Overview 
![Transport Overview](https://github.com/Rutesh18/Telangana_Growth_Analysis/assets/115866652/5db020c1-a594-47a1-999f-17b5b67687af)


# TS-iPass Overview 
![TS-iPass Overview](https://github.com/Rutesh18/Telangana_Growth_Analysis/assets/115866652/c280f7d7-c982-46cb-b964-212a490a07eb)

