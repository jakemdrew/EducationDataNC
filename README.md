# North Carolina Educational Attainment Data Repository
The North Carolina Public Schools Report Card and Statistical Profiles Databases contain a large volume of information about public, charter, and alternative schools in the State of North Carolina. Information that is made publicly accessible comprises data at the school, district, and state levels. This includes statistics on student and school performance, academic growth, diversity, safety, instructor experience levels, school funding, educational attainment, and much more.

# What is Available?
This repository maintains educational attainment data specific to North Carolina Public School Campuses which is organized by academic school year.  All data sources are pulled directly from multiple locations at http://ncpublicschools.org.  This is an open source repository.  All source code is currently written in Python / Pandas / Scikit Learn and published for review via iPython Notebooks.  No programming software or special tools are required to view source code file contents and outputs are each processing stage.  Source code may be viewed in your web browser by clicking on the links in each directory's ReadMe.md content.           


# How is the Data Organized?
**Each academic school year folder contains the following data:**  
* **Raw Datasets** - These are the original data sources provided by http://ncpublicschools.org.  We write code to download each dataset  directly from the original URL, filter by academic school year (when necessary), rename the year and unit_code fields for consistency, and then save the data in its original format prior to any further processing. 
* **School Datasets** - Once each raw data source is filtered by school year and saved in its original format, all files are processed, consolidated, and merged into a single file containing one record per public school campus, per year.  This process is complex and requires multiple table pivots and various other data transformations since many of the original data files contain multiple records per school campus, per year.  Once a master "Public Schools" file is created we also create three additional files with campuses segmented at the high school, middle school, and elementary school levels. We publish all of our source code, so you may click on any of the respective file links to view the original data file URLs and transformations. 
* **Machine Learning Datasets** -  One machine learning (\_ML) dataset is created for each of the School Datasets.  These datasets are intended for modeling and have gone through many additional transformations specific to data pre-processing for machine learning.  This includes removing columns with large amounts of missing data, all unique values, or duplicated / highly correlated columns.  In addition, all categorical variables are converted to numeric data via a process called one-hot encoding.  Specific documentation and transformation reports for each dataset are avaiable in the source code folders.      
# Data Documentation 
* [**data-dictionary.pdf**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/Reports/data-dictionary.pdf) - Metadata file containing field definitions by table for most fields in the NC Report Card database and All_Data_By_School_Final.xlsx

# Reports 
* [**NC Report 2016 Data Overview - MSDS 7331.pdf**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/Reports/NC%20Report%202016%20Data%20Overview%20-%20MSDS%207331.pdf) - Read this to gain a better understanding of what this data is all about!  Overview of NC public school data by Dr. Drew including the current state of majority minority public schools in NC. 

# Acknowledgements
![John M Belk Endowment](http://jmbendowment.org/wp-content/uploads/2015/03/BelkEndowment_-logo-2015.png)

http://jmbendowment.org/
