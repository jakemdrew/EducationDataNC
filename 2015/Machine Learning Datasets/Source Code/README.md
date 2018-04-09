# North Carolina Educational Attainment Data Repository for Machine Learning

The North Carolina Public Schools Report Card and Statistical Profiles Databases contain a large volume of information about public, charter, and alternative schools in the State of North Carolina. Information that is made publicly accessible comprises data at the school, district, and state levels. This includes statistics on student and school performance, academic growth, diversity, safety, instructor experience levels, school funding, educational attainment, and much more.

There were 17 tables of data reviewed within the North Carolina report card database. Two additional tables including racial composition statistics were subsequently located in the statistical profiles database. The current database versions used for this report contain data ranging from 1990-2017. However, not all tables contain data dating back to 1990 or current as of 2017.

Links to the original datasets are listed below.  However, some of these tables have been extensively de-normalized to accommodate visualization and machine learning processes.

# Reports 
* [**data-dictionary.pdf**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/Reports/data-dictionary.pdf) - Metadata file containing field definitions by table for most fields in the NC Report Card database and All_Data_By_School_Final.xlsx
* [**NC Report 2016 Data Overview - MSDS 7331.pdf**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/Reports/NC%20Report%202016%20Data%20Overview%20-%20MSDS%207331.pdf) - Read this to gain a better understanding of what this data is all about!  Overview of NC public school data by Dr. Drew including the current state of majority minority public schools in NC. 

# iPython Notebooks and Code Examples
You can click on each of the notebook names below to preview the code using the [Nbviewer](nbviewer.jupyter.org).
  ## Dataset Creation Notebooks
   * [**Public Elementary Schools Dataset Expanded  Feb 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Dataset%20Creation/Public%20Elementary%20Schools%20Dataset%20Expanded%20%20Feb%202018.ipynb) - Python code to create the ElementarySchoolsML_02_2018_Expanded.csv dataset.  
   * [**Public High Schools Dataset  Feb 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Dataset%20Creation/Public%20High%20Schools%20Dataset%20%20Feb%202018.ipynb) - Python code to create the HighSchoolsML_02_2018.csv dataset.  
   * [**Public High Schools Dataset Expanded  Feb 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Dataset%20Creation/Public%20High%20Schools%20Dataset%20Expanded%20%20Feb%202018.ipynb)  - Python code to create the HighSchoolsML_02_2018_Expanded.csv dataset.  
   * [**Public Middle Schools Dataset Expanded  Feb 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Dataset%20Creation/Public%20Middle%20Schools%20Dataset%20Expanded%20%20Feb%202018.ipynb) - Python code to create the MiddleSchoolsML_02_2018_Expanded.csv dataset.
  
  ## Machine Learning Notebooks 
  * [**Average SAT Scores February 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Average%20SAT%20Scores%20February%202018.ipynb) - This notebook explores predicting the average SAT score for public high schools in North Carolina.
  * [**Elementary School Minority Percentage February 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Elementary%20School%20Minority%20Percentage%20February%202018.ipynb) - This notebook explores predicting the minority racial composition percentage for public elementary schools in North Carolina.
  * [**Graduation Rates February 2018 - 4 Years Expanded.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Graduation%20Rates%20February%202018%20-%204%20Years%20Expanded.ipynb) - This notebook explores predicting the 4 year graduation rates for public high schools in North Carolina.  Data for this notebook is expanded to consider student body racial compositions. 
  * [**Graduation Rates February 2018 - 5 Years Expanded.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Graduation%20Rates%20February%202018%20-%205%20Years%20Expanded.ipynb) - This notebook explores predicting the 5 year graduation rates for public high schools in North Carolina.  Data for this notebook is expanded to consider student body racial compositions.   
  * [**Graduation Rates February 2018 - 4 Years.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Graduation%20Rates%20February%202018%20-%204%20Years.ipynb) - This notebook explores predicting the 4 year graduation rates for public high schools in North Carolina. No student body racial compositions are considered in the training data.    
  * [**Graduation Rates February 2018 - 5 Years.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Graduation%20Rates%20February%202018%20-%205%20Years.ipynb) - This notebook explores predicting the 4 year graduation rates for public high schools in North Carolina. No student body racial compositions are considered in the training data.   
   * [**Graduation Rates v2.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Graduation%20Rates%20v2.ipynb) - Example iPython Notebook with useful code snippets for merging files, isolating high school campuses, and regressing four-year graduation rate within +-4.22 mean absolute error. This notebook also shows how to create your own custom regressor and create multiple scorer functions using the make_scorer() function.  This allows you to perform cross validation one time with the cross_validate() function and return multiple scoring metrics for evaluation (MAE, MAPE, and RMSE in this case).
   * [**Graduation Rates v3.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Graduation%20Rates%20v3.ipynb) – This is the Graduation Rates v2 notebook analysis with the 'Cohort Graduation Rate Standard Score' removed from all training data.
   * [**High School Minority Percentage February 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/High%20School%20Minority%20Percentage%20February%202018.ipynb) - This notebook explores predicting the minority racial composition percentage for public high schools in North Carolina.
   * [**Middle School Minority Percentage February 2018.ipynb**](http://nbviewer.jupyter.org/github/jakemdrew/EducationDataNC/blob/master/iPython%20Notebooks/Machine%20Learning/Middle%20School%20Minority%20Percentage%20February%202018.ipynb) - This notebook explores predicting the minority racial composition percentage for middle schools in North Carolina.

# Machine Learning Dataset and File Descriptions
* [**ElementarySchoolsML_02_2018_Expanded.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Machine%20Learning%20Datasets/ElementarySchoolsML_02_2018_Expanded.csv) - 1291 Public Middle Schools and 136 features prepared for machine learning including racial compositions for each campus.
* [**MiddleSchoolsML_02_2018_Expanded.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Machine%20Learning%20Datasets/HighSchoolsML_02_2018.csv) - 535 Public Middle Schools and 128 features prepared for machine learning including racial compositions for each campus.
* [**HighSchoolsML_02_2018_Expanded.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Machine%20Learning%20Datasets/HighSchoolsML_02_2018_Expanded.csv) - 440 Public High Schools and 140 features prepared for machine learning including racial compositions for each campus.
* [**HighSchoolsML_02_2018.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Machine%20Learning%20Datasets/MiddleSchoolsML_02_2018_Expanded.csv) - 440 Public High Schools and 128 features prepared for machine learning.  

# Raw Dataset and File Descriptions
* [**All_Data_By_School_Final.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Raw%20Datasets/All_Data_By_School_Final.csv) - 2575 records, 293 fields - One record for each active public school in the State of North Carolina.  Features reflect school level attributes.  Data is consolidated from various tables within the NC Statistical Profiles and Report Card Databases.  (See download links below)  The following formula was applied to each cell in Excel to remove masking and clean up this data for processing = TRIM(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(Sheet1!A2,"*","0"),">95","100"),"<5","0"),"<10","5"),"""",""),",",""))  
* [**Ec_Pupils_Expanded (2017 Race Compositions by School).csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Raw%20Datasets/Ec_Pupils_Expanded%20(2017%20Race%20Compositions%20by%20School).csv) - 2447 records, 30 fields, racial composition data for each active public school in the state of North Carolina (minus charter schools and vocational schools).  See Table 11 - A HISTORY OF PUPIL MEMBERSHIP BY RACE below for original links.    
* [**accdrilldwn16_masking_removed.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Raw%20Datasets/accdrilldwn16_masking_removed.csv) - 84950 records, 32 fields -  Percentages of students within each public school by race passing numerous educational attainment performance metrics. (i.e. Graduation Rates, SAT, ACT, End of Year (EOY), and End of Course (EOC) by grade). The following formula was applied to each cell in Excel to clean up this data for processing = TRIM(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(Sheet1!A2,"*","0"),">95","100"),"<5","0"),"<10","5"),"""",""),",","")) 
* [**1516testresults_masking_removed.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Raw%20Datasets/1516testresults_masking_removed.csv) - 39857 records, 12 fields - Percentages of students within each public school passing numerous educational attainment performance metrics broken out in levels 1 - 5.  (i.e. Graduation Rates, SAT, ACT, End of Year (EOY), and End of Course (EOC) by grade). The following formula was applied to each cell in Excel to clean up this data for processing = TRIM(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(Sheet1!A2,"*","0"),">95","100"),"<5","0"),"<10","5"),"""",""),",","")) 
* [**1516_Test_Scores.xlsx**](https://github.com/jakemdrew/EducationDataNC/blob/master/Raw%20Datasets/1516_Test_Scores.xlsx) - 2669 records, 73 fields - Percentage of entire student body meeting various subject or test End of Grade (EOG), End of Course (EOC), ACT and Graduation Rate benchmarks.  This data was transformed to one record per school from the accdrilldwn16_masking_removed.csv file. The accdrilldwn16_masking_removed.csv file also contains these same percentages by race.   The following acronyms also help to decipher field meanings: 
  * EOC - End of Course
  * EOG - End of Grade
  * CACR - College and Career Ready  
 * [**1516_Test_Scores.csv**](https://github.com/jakemdrew/EducationDataNC/blob/master/Raw%20Datasets/1516_Test_Scores.csv) - A .csv version of 1516_Test_Scores.xlsx.

# Links to Original Data

**These links are for reference only!  Most features have been consolidated into the file All_Data_By_School_Final.xlsx.  However, you may find additional data here if it is missing.**  

## Reseracher Download Page:

http://www.ncpublicschools.org/src/researchers/

## Download Links:

Data Dictionary:
http://www.ncpublicschools.org/docs/src/researchers/data-dictionary.pdf

## Combined Zip File:
http://www.ncpublicschools.org/docs/src/researchers/src-combined.zip

## Profile Table:
School Profile -> School Information/School Size
http://www.ncpublicschools.org/docs/src/researchers/profile.xlsx

## Profile Metrics Table:
School Profile -> Average Class Size
http://www.ncpublicschools.org/docs/src/researchers/profile-metrics.xlsx

## Funding Table:
District Profile -> Funding
http://www.ncpublicschools.org/docs/src/researchers/funding.xlsx

## School Performance Grade Table: 
School Performance -> School Performance Grade
http://www.ncpublicschools.org/docs/accountability/reporting/spg1415.xlsx

## READY Accountability Tables:
School Performance -> EOG/EOC/The ACT/ACT WorkKeys/Passing Math III/Cohort Grad Rate
http://www.ncpublicschools.org/docs/accountability/reporting/accdrilldwn16.xlsx
http://www.ncpublicschools.org/docs/accountability/reporting/1516testresults.xlsx

## Read to Achieve Table
School Performance -> Read to Achieve
http://www.ncpublicschools.org/docs/src/researchers/rta.xlsx

## Participation Targets Overall Table 
School Performance -> Participations Targets
http://www.ncpublicschools.org/docs/accountability/reporting/participation-targets.xlsx  (NOT AVAILABLE)

## School Indicators Table 
School Indicators -> SAT/AP/IB
http://www.ncpublicschools.org/docs/src/researchers/school-indicators.xlsx


## Advanced Placement Courses
School Indicators -> AP
http://www.ncpublicschools.org/docs/src/researchers/ap-courses.xlsx

## Specialized Course Enrollment Table
School Indicators -> Specialized Course Enrollment
http://www.ncpublicschools.org/docs/src/researchers/sce.xlsx

## College Enrollment Table
School Indicators -> College Enrollment
http://www.ncpublicschools.org/docs/src/researchers/college-enrollment.xlsx

## College Course Completion Table
School Indicators -> College Course Enrollment
http://www.ncpublicschools.org/docs/src/researchers/college-enrollment-completion.xlsx

## Environment Table
School Environment -> Attendance/Digital Learning Devices/Safety
http://www.ncpublicschools.org/docs/src/researchers/environment.xlsx

## Personnel Table 
Personnel -> Classroom Teachers/Licenses/Highly Qualified/Teachers with Advanced Degrees/NBCT/Teacher Turnover
http://www.ncpublicschools.org/docs/src/researchers/personnel.xlsx

## National Assessment of Educational Progress (NAEP)
State Report Card
http://www.ncpublicschools.org/docs/src/researchers/naep.xlsx

## Educator Experience
Personnel -> Teacher/Principal Experience
http://www.ncpublicschools.org/docs/src/researchers/yoe.xlsx

## Educator Effectiveness
Personnel -> Teacher and Administrator Effectiveness
http://www.ncpublicschools.org/docs/src/researchers/effectiveness.xlsx


## Additional Data:

http://www.ncpublicschools.org/data/reports/


## Statistical Profile Data Tables:

Homepage:
http://www.ncpublicschools.org/fbs/accounting/data/

## Statistical Profiles App:
http://apps.schools.nc.gov/ords/f?p=145:2:::NO:::

## Table 10.1 - PUPILS IN MEMBERSHIP BY RACE and SEX (at School Level) 2011-2017
http://apps.schools.nc.gov/ords/f?p=145:16:::NO::


## Table 10 - Pupils in Membership by Race & Sex 2004-2010 (at district level)
http://apps.schools.nc.gov/ords/f?p=145:16:::NO::


## Table 11 - A HISTORY OF PUPIL MEMBERSHIP BY RACE

## Statewide Data 1989 - 2010
http://apps.schools.nc.gov/ords/f?p=145:16::FLOW_XMLP_OUTPUT_R433132594546366325_en-us::::&cs=3s8ZhtbU6wIHVEyb2E4zG8n88n-1lqYNykxx4H9vAfcg7LiFankc0UM5WhGg1uSf_t_4qxeSbuJYqvyV9nGZHVQ

## Statewide Data 2010 - 2017
http://apps.schools.nc.gov/ords/f?p=145:16::FLOW_XMLP_OUTPUT_R488359791967292919_en-us::::&cs=3ykPh3YYGy33OCxL3expOsbhKoRNg2OBzs-5DbFhTjjTF9wrIr3XqzSDLbzFSAh3Zvmc0I7G5egrt6VAdGTNjAw
