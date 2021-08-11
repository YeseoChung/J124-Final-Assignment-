# J124 Final Project

Datasets I worked with are: 
* "Student Data" which deals with data related to vaccinations and exemptions for incoming kindergarteners from school years 2000-2001 through 2014-2015. 
* "pertussisRates_2010_2015" which outlines pertussis rates by county between 2010 and 2015. 

**Which county had the highest number of PBE(Personal belief exemption)?**
1. Create pivot table with "County" as row and "Sum of nPBE" as value.
2. Copy entire pivot table and paste into new sheet as "values only."
3. Sort "nPBE" column from "Z to A" to find the highest number of personal belief exemptions. <br/>
_Los Angeles County had the highest number of PBE(Personal belief exemptions) with 24,015._

!['Question1','pivotTable'](/Question1.jpg)

**Which county had the highest number of PME(Permanent medical exemption)?**
1. Create pivot table with "County" as row and "nPME" as value. 
2. Copy entire pivot table and paste into new sheet as "values only."
3. Sort "nPME" column from "Z to A" to find the highest number of permanent medical exemptions.
_Los Angeles County had the highest numer of permanent medical exemptions with 2,376._

!['Question1','pivotTable'](/Question2.jpg)

**What percent of each county had PBE in 2014?**
1. Use filter tool to show just data for 2014. 
2. Copy data for 2014 into new sheet. 
3. Use 2014 data to create pivot table with "County" as row and "Sum of n" and "Sum of nPBE" as values. 
4. Copy pivot table into new sheet and paste as "values only." 
5. Use division formula to find percent of PBE in each county. In other words, I am dividing number of PBE of each county by the total number of incoming kindergarteners. 
6. Sort the "percentage of PBE" from "Z-A"(in descending order)
7. The chart below illustrates my findings: 

!['Question1','pivotTable'](/Question3.jpg)

**What percent of each county had PME in 2014?**
1. Use filter tool to show just data for 2014. 
2. Copy data for 2014 into new sheet. 
3. Use 2014 data to create pivot table with "County" as row and "Sum of n" and "Sum of nPME" as values. 
4. Copy pivot table into new sheet and paste as "values only." 
5. Use division formula to find percent of PBE in each county. I am dividing the number of PMEs in each county by the total number incoming kindergarteners to find the percentage. 
6. Sort the "percentage of PME" from "Z-A" (in descending order)
7. The chart below illustrates my findings: 

!['Question1','pivotTable'](/Question4.jpg)

**What is the percent change between 2000 and 2015 for DTP vaccinations?**
* Please note that percent change could not be calculated for Alpine county because data is only available between 2000 and 2013 for Alpine county.
1. Pivot table. Row as "County." Value as "nDTP."
2. Use filter to isolate this pivot table for 2000. Copy this data into new sheet as "values only."
3. Use filter on pivot table again to isolate data for 2015. Copy "nDTP" for 2015 into the new sheet. 
4. Use percent change formula which is (New-Old/Old X 100) to find percent change. 
5. Sort percent change of DTP from "Z-A"(in descending order). 
6. The chart below illustrates my findings:

!['Question1','pivotTable'](/Question5fixed.jpg)

**What is the percent change between 2000 and 2013 for DTP vaccinations in Alpine County?**
1. Pivot table. Row as "County." Value as "nDTP."
2. Use filter to isolate this pivot table for just Alpine County.
3. Then use another filter to just show the year 2000. Copy this data into new sheet as "values only."
4. Use filter on pivot table again to isolate data for just 2013. Copy "nDTP" for 2013 into the new sheet. 
5. Use percent change formulato find percent change. 
6. Sort "percent change of DTP" from "Z-A"(in descending order). 
7. The chart below illustrates my findings:
8. 

**Using "pertussisRates_2010_2015" identify which year had the highest number of pertussis cases.**
1. The dataset had a total count and rate of pertussis for the entire state of california. 
2. Between 2010 and 2014, the year with the highest number of pertussis in California was in 2014. 
