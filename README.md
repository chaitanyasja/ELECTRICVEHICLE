# ELECTRICVEHICLE
# **Electric Vehicle Dashboard**

### **Dashboard Link** : https://app.powerbi.com/links/9_R_PFXhtG?ctid=e59bad41-e823-45c9-b8d1-c55bd714b9ae&pbi_source=linkShare

## Problem Statement



![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/e7a6f55b-1c87-413c-b618-dd8765d6e093)

 **Total Vehicles:**
Understand the overall landscape of electric vehicles, encompassing both BEVs and PHEVs, to assess the market's size and growth.
2. Average Electric Range:
Determine the average electric range of the electric vehicles in the dataset to gauge the technological advancements and efficiency of the EVs.
3. Total BEV Vehicles and % of Total BEV Vehicles:
Identify and analyze the total number of Battery Electric Vehicles (BEVs) in the dataset.
Calculate the percentage of BEVs relative to the total number of electric vehicles, providing insights into the dominance of fully electric models.
4. Total PHEV Vehicles and % of Total PHEV Vehicles:
Identify and analyze the total number of Plug-in Hybrid Electric Vehicles (PHEVs) in the dataset.
Calculate the percentage of PHEVs relative to the total number of electric vehicles, offering insights into the market share of plug-in hybrid models.



### Steps followed 

- Total Vehicles by Model Year (From 2010 Onwards):
Visualization: Line/ Area Chart
Description: This chart will illustrate the distribution of electric vehicles over the years, starting from 2010, providing insights into the growth pattern and adoption trends.
2. Total Vehicles by State:
Visualization: Map Chart 
Description: This chart will showcase the geographical distribution of electric vehicles across different states, allowing for the identification of regions with higher adoption rates.
3. Top 10 Total Vehicles by Make:
Visualization: Bar Chart 
Description: Highlight the top 10 electric vehicle manufacturers based on the total number of vehicles, providing insights into the market dominance of specific brands.
4. Total Vehicles by CAFV Eligibility:
Visualization: Pie Chart or Donut Chart
Description: Illustrate the proportion of electric vehicles that are eligible for Clean Alternative Fuel Vehicle (CAFV) incentives, aiding in understanding the impact of incentives on vehicle adoption.
5. Top 10 Total Vehicles by Model:
Visualization: Tree map
Description: Highlight the top 10 electric vehicle models based on the total number of vehicles, offering insights into consumer preferences and popular models in the market.


       

        
- Step 15 : New measure was created to find total 

Following DAX expression was written ,

**1.
        Avg Range = CONCATENATE(FORMAT(AVERAGE(Electric_Vehicle_Population_Data[Electric Range]),"0.00"),"KM")**

**2. bevewhicles = CALCULATE([Total Vehicles],Electric_Vehicle_Population_Data[Electric Vehicle Type] = "Battery Electric Vehicle (BEV)" )** 

**3.   Perc of BEV = [bevewhicles]/[Total Vehicles]**  

**4.Perc of PHEV = [Phevehicles]/[Total Vehicles]**

**5.Phevehicles = CALCULATE([Total Vehicles],Electric_Vehicle_Population_Data[Electric Vehicle Type] = "Plug-in Hybrid Electric Vehicle (PHEV)" )**

**6.Total Vehicles = DISTINCTCOUNT(Electric_Vehicle_Population_Data[DOL Vehicle ID])**

 
 - Step 17 : New measure was created to calculate total distance travelled by flights & a card visual was used to represent total distance.
 
 Following DAX expression was written to find total distance,
 
         Total Distance Travelled = SUM(airline_passenger_satisfaction[Flight Distance])
    
 
 

 
 # Report Snapshot (Power BI DESKTOP)


![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/3bb0c9e7-a2c1-4a26-a6c8-500f5f50c2e0)



# Insights


![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/51b73695-88a6-48f8-af45-ea0d56f5ca0b)



![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/9b343942-c48a-4f1a-a3d0-603856a34c28)




![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/d9a330ed-3566-4222-94b0-b642525f3b0a)


![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/5f1abb08-9726-4ee9-80f2-1b4a57a5441a)



![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/6087bd4e-9696-420e-8bfb-87f8fd4e1df2)



![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/ed3a3166-c1b2-4c22-b3aa-c9a6273b427b)



![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/afde430e-5bfe-400c-98a8-6f00fee7b5a9)



![Image](https://github.com/users/chaitanyasja/projects/3/assets/114214825/2b880955-7f9e-4889-923b-30460499285c)
