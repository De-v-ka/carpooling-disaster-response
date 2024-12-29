# **Coordinated Carpooling for Disaster Response**

This repository contains a Python-based simulation for coordinating carpooling to evacuate disaster victims to nearby shelters efficiently.

## **Features**
- **Victim and Shelter Data Generation**: Randomly generates victim and shelter data using the `Faker` library.
- **Spatial Clustering**: Uses DBSCAN to cluster victims based on their proximity to each other.
- **Shelter Assignment**: Calculates distances between victims and shelters, assigning victims to the nearest shelter.
- **Transport Grouping**: Groups victims into transport units based on proximity and shelter capacity.
- **Interactive Map**: Visualizes the transport routes between victims and shelters using `Folium`, with color-coded lines for different carpool groups.

## **How It Works**
1. **Data Generation**: 
   - Victim data, including location, urgency, and priority needs, is randomly generated using the `Faker` library, and shelter locations are predefined.
2. **Clustering**: 
   - DBSCAN is used to group victims based on their proximity to each other.
3. **Shelter Assignment**: 
   - Victims are assigned to the nearest shelter based on distance, and transport groups are formed based on shelter capacity.
4. **Map Visualization**: 
   - An interactive map is generated using `Folium`, showing victims, shelters, and transport routes. Different transport groups are represented with color-coded lines.

## **Setup and Usage**
### **Prerequisites**
- Python 3.6+
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `folium`, `geopy`, `Faker`, `matplotlib`

Install the required libraries using:
```bash
pip install pandas numpy scikit-learn folium geopy Faker matplotlib
