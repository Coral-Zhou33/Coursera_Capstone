# The Battle of Neighborhoods - New York
### 1. Introduction/Business Problem
### 2. Data Requirment
### 3.Methodology

## Introduction/Business Problem

This project is talking about the neighborhoods of New York. The major Target Audience would be business owners and stake holders who planning to start a Middle and high class  Italian restaurant in New York, this project would help them find the optimal location.  
The Foursquare API is used to access the venues in the neighborhoods. Since, it returns less venues in the neighborhoods, we would be analysing areas for which countable number of venues are obtained. Then they are clustered based on their venues using Data Science Techniques.

1. Due to the high cost of restaurant, this area should be one of the regions with high employment and high imcomes.
2. Hope as many consumers as possible patronize the restaurant, so there should be a large and dense population nearby.
3. Since this is an Italian restaurant, stay away from Italian restaurant as much as possible and in areas with high dining popularity.
4. Tourists and business travelers have high spending power, so it's important to close to the hotel, and not too far from the city center or other tourist hotspots.
5. To ensure the safety of constomers and restaurant staff, select a low-risk area.

## Data Requirment
1. In order to obtain the venue details in each neighborhood of New York City, Foursquare API is used. <br>
     [https://foursquare.com/](https://foursquare.com/)
   * Borough
   * Neighborhood	
   * Latitude
   * Longitude
   * Venue Category data
   
   id| Borough   | Neighborhood |	Latitude	| Longitude
   --|---------  |--------------|------------|-------------
   0 |	Bronx  |	Wakefield	  | 40.894705	|-73.847201
   1 |	Bronx  |	Co-op City  | 40.874294	|-73.829939
   2 |	Bronx  |	Eastchester | 40.887556	|-73.827806
   3 |	Bronx  |	Fieldston	  | 40.895437	|-73.905643
   4 |	Bronx  |	Riverdale	  | 40.890834	|-73.912585

     Name       |  Categories   | Lat         | Lng
   -------------|-------------- |-------------|-------------
   Bikram Yoga  |	Yoga Studio |	40.876844	 | -73.906204
   Arturo's     | Pizza Place   |	40.874412	 | -73.910271
   Tibbett Diner|	Diner	  | 40.880404	 | -73.908937
   Dunkin'	 | Donut Shop    | 40.877136	 | -73.906666
   Starbucks    |	Coffee Shop |	40.877531  | -73.905582


2. Acquire the other data as follows: <br>
    [https://data.cccnewyork.org/data](https://data.cccnewyork.org/data)  <br>
    [wikipedia.org/wiki/Boroughs_of_New_York_City](https://em.m.wikipedia.org/wiki/Boroughs_of_New_York_City) <br>
   * The population density of the boroughs of New York City
   * Number of people in each New York Community
   * New York City Community Employment Rate
   * Median household income level
   * New York City reported felony rates
   * Community trust
 
 
   COMMUNITY DISTRICTS | Total Population         
   --------------------|---------------------------
   Astoria(Q01)	     | 166,069
   Battery Park/Tribeca(M01) | 66,438
   Bay Ridge(K10)  	| 121,925
   Bayside(Q11)	     | 114,562
   Bedford Park(B07)	| 151,684


   COMMUNITY DISTRICTS | Employment Rate
   --------------------|----------------------------
   Astoria(Q01)	     | 69.0%
   Battery Park/Tribeca(M01) | 73.3%
   Bay Ridge(K10)	     | 58.1%
   Bayside(Q11)	     | 59.7%
   Bedford Park(B07)	| 61.4%

   COMMUNITY DISTRICTS | All Households
   --------------------|----------------------------
   Astoria(Q01)	   | $79,180	
   Battery Park/Tribeca(M01) | $162,092	
   Bay Ridge(K10)	   | $76,569	
   Bayside(Q11)	   | $92,682	
   Bedford Park(B07)   |$41,336

   COMMUNITY DISTRICTS |  Violent Felonies
   --------------------|----------------------------
   Astoria(Q01)    	   | 4.3
   Battery Park/Tribeca(M01) | 2.7
   Bay Ridge(K10) 	   | 1.6
   Bayside(Q11)	   | 0.9
   Bedford Park(B07)   | 5.9

   COMMUNITY DISTRICTS | Community Trust
   --------------------|----------------------------
   Astoria(Q01)	   | 73.0%
   Battery Park/Tribeca(M01)  | 70.0%
   Bay Ridge(K10)	   | 74.0%
   Bayside(Q11)	   | 86.0%
   Bedford Park(B07)   | 63.0%
   
