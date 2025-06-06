# Deloitte_Internship

### Project Overview
This project is by Deloitte Job Simulation found on The Forage (https://www.theforage.com/
Deloitte has a client named Daikibo who has factories in four different locations. Each location has 9 different types of machines, sending a message every 10 minutes. Daikibo has been collecting this data for one month (May 2021) and they've shared this data in the form of a single JSON file. My task seeks to answer 2 questions by the client
1. In which location did machines break the most?
2. What are the machines that broke most often in the location?

### Data Sources
Daikobo telementary Data: The primary dataset used for this analysis is the "daikobo-telementary-data.json" file containing detailed information about each location and machine owned by the company over a period of 1 month.

### Tools Used
- Tableau Public (for visualizing data)

### Process
- I imported the JSON file into Tableu and selected all Schema Levels.
- I then clicked on Create Calculated Field which led to a dialogue box for renaming and calculation code.
- I named the field Unhealthy and used the formula;
  ```
  IF[Status}="Unhealthy"
  THEN 10
  ELSE 0
  END
  ```
- I then created a "Downtime Per Factory" chart which helped us identify the number of machine breakdowns per factory.
- I then created a "Downtime Per Machine" chart which helped us identify which machines broke down the most per factory.
- Finally, I synced the two charts and added a filter in the factory chart so that the bottom chart can show the downtime of all machines per factory.
