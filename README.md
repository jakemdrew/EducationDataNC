# EducationDataNC

The North Carolina Public Schools Report Card and Statistical Profiles Databases contain a large volume of information about public, charter, and alternative schools in the State of North Carolina. Information that is made publicly accessible comprises data at the school, district, and state levels. This includes statistics on student and school performance, academic growth, diversity, safety, instructor experience levels, school funding, educational attainment, and much more.

There were 17 tables of data reviewed within the North Carolina report card database. Two additional tables including racial composition statistics were subsequently located in the statistical profiles database. The current database versions used for this report contain data ranging from 1990-2017. However, not all tables contain data dating back to 1990 or current as of 2017.

Links to the original datasets are listed below.  However, some of these tables have been extensively de-normalized to accommodate visualization and machine learning processes.

# Dataset and File Descriptions

* **All_Data_By_School_Final.xlsx** - 2575 records, 293 fields - One record for each active public school in the State of North Carolina.  Features reflect school level attributes.  Data is consolidated from various tables within the NC Statistical Profiles and Report Card Databases.  (See download links below)
* **data-dictionary.pdf** - Metadata file containing field definitions by table for most fields in the NC Report Card database and All_Data_By_School_Final.xlsx
* **Ec_Pupils_Expanded (2017 Race Compositions by School).csv** - 2447 records, 30 fields, racial composition data for each active public school in the state of North Carolina (minus charter schools and vocational schools).  See Table 11 - A HISTORY OF PUPIL MEMBERSHIP BY RACE below for original links.   
* **NC Report 2016 Data Overview - MSDS 7331.pdf** - Read this to gain a better understanding of what this data is all about!  Overview of NC public school data by Dr. Drew including the current state of majority majority public schools in NC.
* **ReadMe.txt** - Links to all original data.  This information is also included directly below.   
* **accdrilldwn16_masking_removed.csv** - 84950 records, 32 fields -  Percentages of students within each public school by race passing numerious educaitonal attainment performance metrics. (i.e. Graduation Rates, SAT, ACT, End of Year (EOY), and End of Course (EOC) by grade). The following formula was applied to each cell in Excel to clean up this data for processing = TRIM(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(Sheet1!A2,"*","0"),">95","100"),"<5","0"),"<10","5"),"""",""),",","")) 
* **1516testresults_masking_removed.csv** - 39857 records, 12 fields - Percentages of students within each public school passing numerious educaitonal attainment performance metrics broken out in levels 1 - 5.  (i.e. Graduation Rates, SAT, ACT, End of Year (EOY), and End of Course (EOC) by grade). The following formula was applied to each cell in Excel to clean up this data for processing = TRIM(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(SUBSTITUTE(Sheet1!A2,"*","0"),">95","100"),"<5","0"),"<10","5"),"""",""),",","")) 
* **1516_Test_Scores.xlsx** - 2669 records, 73 fields - Percentage of entire student body meeting various subject or test End of Grade (EOG), End of Course (EOC), ACT and Graduation Rate benchmarks.  This data was transformed to one record per school from the accdrilldwn16_masking_removed.csv file. The accdrilldwn16_masking_removed.csv file also contains these same percentages by race.   The following acronyms also help to decipher field meanings: 
  * EOC - End of Course
  * EOG - End of Grade
  * CACR - College and Career Ready         

# Links to Original Data

These links are for reference only!  Most features have been consolidated into the file All_Data_By_School_Final.xlsx.  However, you may find additional data here if it is missing.  

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
