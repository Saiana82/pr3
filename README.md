# Wildfire Analysis

![image](https://i.pinimg.com/originals/ec/85/10/ec85104066682a9397972283cc5badf5.jpg)

## Table of Contents
   =================

  1. [About This Project](#about-this-project) <br>
	 - [Architectural Diagram](#architectural-diagram)
  	 - [ETL Process](#etl-process)
  4. [Visualizations](#visualizations)
  5. [Deployment](#deployment)
  6. [Contributors](#contributors)

## About This Project 	
Our team was interested in exploring wildfire data. We extracted wildfire data across the United States to create an engagine and informative visualization of all wildfires that occurred in 2021. Data was extracted from CSV source, transformed using Python, Pandas and SQL. Data was then loaded into PostgreSQL. Visualizations was done using JavaScript, Matplotlib, Leaflet, Folium, Python, Flask, HTML, CSS. Heroku was used to deploy results to a 2021 wildfire web application. 


## Architectural Diagram 	
<img src="https://i.pinimg.com/564x/f8/3e/a0/f83ea0cb3e44c82cf020dd4803eb979b.jpg" width=800 align=center> <br>

## ETL Process 	

#### Extract 
2021 Wildfire dataset was extracted from the [National Interagency Fire Center](https://data-nifc.opendata.arcgis.com/datasets/wfigs-2021-wildland-fire-perimeters-to-date/explore?location=0.000000%2C0.000000%2C0.00&showTable=true).

	- Format: CSV
	- Size:  KB

#### Transform 
Data was transformed and cleaned using Python, Pandas with th Jupyter Notebook. 
Transformations include: 
- Filtering dataframe for year = 2021.   
- Changing column datatypes
- Renaming columns
- Retrieving required columns and dropping unwanted columns to load into PostgreSQL		

#### Load
The clean data was imported into a pgAdmin Data Base using PostgeSQL from where it can be extracted for future analysis. 


### Visualizations 	
## Top 20 States by Wildfires: <br>
Grouping by state, it can be concluded that majority of wildfires incidents happen in a couple of states, with Montanta, Idaho, and Arizona being on the top of the list, respectively. Suprisingly, California comes in fourth, with Montana having more then twice the amount of incidents


<img src="https://i.pinimg.com/236x/93/88/bf/9388bfbd0c8147a957585beea0043228.jpg" width=400 align=center> <br>

## Acres Burned vs Duration: <br>
Wildfires burned more acres the longer the duration of the fire in the beginning stage of the fire. Most of the fires, after around 20 days, were subdued and under control with only a handful still increasing in the size of acres burned. After 100 days, all fires in our dataset were under control with minimal burning.


<img src="https://i.pinimg.com/564x/b7/d0/c7/b7d0c7a71dc28b1d1ffe1f9a3e48285d.jpg" width=600 align=center> <br> 

## Wildfires by Month: <br>
Looking at the data grouped by month, We can clearly see that the number of wildfires in winter is relatively low and that it significantly increases in the summer, especially in June and July

<img src="https://i.pinimg.com/originals/83/c8/4d/83c84d102ec307e097a17e299e65bf51.jpg" width=600 align=center> <br> 

## Top Causes: <br>
Tree Map with the top causes of wildfires shows us that the biggest cause of wildfires lighting. For a good chunk of it, the cause of the fire is not known.

<img src="https://i.pinimg.com/564x/3a/9e/22/3a9e22fde630dc6bf282908f087f71c6.jpg" width=600 align=center> <br> 

## Deployment

A home HTML file that links to a charts HTML and data HTML files, were created to display the data and its findings in the HTML format on the web.
CSS/Bootstrap are used to style the webpages.
A flask app.py file was created as a micro web framework to deploy the web application hosted by Heroku as well as on GitHub.

## Contributors

- [Ranjani Venkatraman](https://github.com/RanjaniAnjurVenkatraman)
- [Novak Radovic](https://github.com/nradovic1)
- [Saiana Darizhapova](https://github.com/Saiana82)
- [David Owens](https://github.com/)


	
