# The Belk Endowment Educational Attainment Data Repository for North Carolina Public Schools
The North Carolina Public Schools Report Card and Statistical Profiles Databases contain a large volume of information about public, charter, and alternative schools in the State of North Carolina. Information that is made publicly accessible comprises data at the school, district, and state levels. This includes statistics on student and school performance, academic growth, diversity, safety, instructor experience levels, school funding, educational attainment, and much more.

# What is Available?
This repository maintains educational attainment data specific to North Carolina Public School Campuses which is organized by academic school year.  All data sources are pulled directly from multiple locations at http://ncpublicschools.org.  This is an open source repository.  All source code is currently written in Python / Pandas / Scikit Learn and published for review via iPython Notebooks.  No programming software or special tools are required to view source code file contents and outputs are each processing stage.  Source code may be viewed in your web browser by clicking on the links in each directory's ReadMe.md content.           


# How is the Data Organized?
**Each academic school year folder contains the following data:**  
* **Raw Datasets** - These are the original data sources provided by http://ncpublicschools.org.  We write code to download each dataset  directly from the original URL, filter by academic school year (when necessary), rename the year and unit_code fields for consistency, and then save the data in its original format prior to any further processing. 
* **School Datasets** - Once each raw data source is filtered by school year and saved in its original format, all files are processed, consolidated, and merged into a single file containing one record per public school campus, per year.  This process is complex and requires multiple table pivots and various other data transformations since many of the original data files contain multiple records per school campus, per year.  Once a master "Public Schools" file is created we also create three additional files with campuses segmented at the high school, middle school, and elementary school levels. We publish all of our source code, so you may click on any of the respective file links to view the original data file URLs and transformations at each processing stage. 
* **Machine Learning Datasets** -  One machine learning (\_ML) dataset is created for each respective public school dataset.  These datasets are intended for classification or regression modeling and have gone through many additional transformations specific to data pre-processing for machine learning.  This includes removing columns with large amounts of missing data, all unique values, or duplicated / highly correlated columns.  In addition, all categorical variables are converted to numeric data via a process called one-hot encoding.  Specific documentation and transformation reports for each dataset are avaiable in the source code folders.

# Data Documentation 
**The following resources and reports are currently available to assist in understanding table, field, and code definitions for public school data:**
* [**data-dictionary.pdf**](https://github.com/jakemdrew/EducationDataNC/blob/master/Data%20Documentation/data-dictionary.pdf) - Metadata file containing field definitions by table for most fields in the NC Report Card database and All_Data_By_School_Final.xlsx

# Reports 
**This folder includes links to research and reports produced using data in this repository.** 
* Brown et. al., [**Postsecondary Attainment: Identifying Areas to Improve Retention for North Carolina Community Colleges**]( https://github.com/jakemdrew/EducationDataNC/blob/master/Reports/Postsecondary%20Attainment.pdf), SMU Data Science Review, 04/2019.
* Brown et. al., [**Presentation Slides - Postsecondary Attainment: Identifying Areas to Improve Retention for North Carolina Community Colleges**]( https://github.com/jakemdrew/EducationDataNC/blob/master/Reports/NBrown_JHeinen_MRega_LSterling_Symposium_Presentation.pdf), SMU Data Science Review, 04/2019.
* Brown et. al., [**Presentation Video - Postsecondary Attainment: Identifying Areas to Improve Retention for North Carolina Community Colleges**]( https://www.youtube.com/watch?v=TvW91hBuzxY&t=1s), SMU Data Science Immersion, 04/2019.
* Drew et. al., [**Reverse Engineering Segregation in North Carolina Public Schools**]( https://github.com/jakemdrew/EducationDataNC/blob/master/Reports/Reverse_Engineering_Segregation_in_North_Carolina_Public_Schools%2010_2018.pdf), 10/2018.
* Leeson et. al., [**Identifying Areas for Change: A Case Study on North Carolina State Public School Performance**]( https://github.com/jakemdrew/EducationDataNC/blob/master/Reports/Identifying%20Areas%20for%20Change_%20NC%20Public%20School%20Performance.pdf), SMU Data Science Review, 08/2018.
* Leeson et. al., [**Presentation Slides - Identifying Areas for Change: A Case Study on North Carolina State Public School Performance**]( https://github.com/jakemdrew/EducationDataNC/blob/master/Reports/KBean_OLeeson_SymposiumLighteningTalk.pdf), SMU Data Science Immersion, 08/2018.
* Leeson et. al., [**Presentation Video - Identifying Areas for Change: A Case Study on North Carolina State Public School Performance**]( https://www.youtube.com/watch?v=07wpQZ7dCuU), SMU Data Science Immersion, 08/2018.
* Leeson et. al., [**Poster - Identifying Areas for Change: A Case Study on North Carolina State Public School Performance**]( https://github.com/jakemdrew/EducationDataNC/blob/master/Reports/KBean_OLeeson_SymposiumPosterPresentation.pdf), SMU Data Science Immersion, 08/2018.
* Drew, Jake, [**2016-2017 North Carolina Public Schools Educational Attainment Data Overview**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/Reports/NC%20Report%202016%20Data%20Overview%20-%20MSDS%207331.pdf), 01/2018. 

# Citations
**Please cite this repository and send us an email, if you use it!**

## References
Drew J., The Belk Endowment Educational Attainment Data Repository for North Carolina Public Schools, (2018), GitHub repository, https://github.com/jakemdrew/EducationDataNC

## BibTeX 
@misc{BelkNCEARepo,  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;author = {Drew, J.},  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title = {The Belk Endowment Educational Attainment Data Repository for North Carolina Public Schools},  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;year = {2018},  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;publisher = {GitHub},  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;journal = {GitHub repository},  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;howpublished = {\url{https://github.com/jakemdrew/EducationDataNC}}  
}  

# Acknowledgements
![John M Belk Endowment](http://jmbendowment.org/wp-content/uploads/2015/03/BelkEndowment_-logo-2015.png)

This research is made possible by: http://jmbendowment.org/
