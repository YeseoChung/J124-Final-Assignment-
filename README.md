# J124 Final Project

Datasets I worked with are: 
* "Student Data" which deals with data related to vaccinations and exemptions for incoming kindergarteners from school years 2000-2001 through 2014-2015.
  * n= number of students 
  * nDTP= number of DTP vaccinations
  * nPBE= number of personal belief exemptions 
  * nPME= numbe of permanent medical exemptions 
* "pertussisRates_2010_2015" which outlines pertussis rates by county between 2010 and 2014. 

## Data Analysis Questions

**Which county had the highest number incoming kindergarteners with PBE(Personal belief exemption)?**
1. Create pivot table with "County" as row and "SUM of nPBE" as value.
2. Copy entire pivot table and paste into new sheet as "values only."
3. Sort "nPBE" column from "Z to A" to find the highest number of personal belief exemptions. <br/>
_Los Angeles County had the highest number of PBE(Personal belief exemptions) with 24,015._

!['Question1','pivotTable'](/Question1.jpg)

**Which county had the highest number of incoming kindergarteners with PME(Permanent medical exemption)?**
1. Create pivot table with "County" as row and "SUM of nPME" as value. 
2. Copy entire pivot table and paste into new sheet as "values only."
3. Sort "nPME" column from "Z to A" to find the highest number of permanent medical exemptions.
_Los Angeles County had the highest numer of permanent medical exemptions with 2,376._

!['Question1','pivotTable'](/Question2.jpg)

**What percent of incoming kindergarteners in each county had PBE in 2014?**
1. Use filter tool to show just data for 2014. 
2. Copy data for 2014 into new sheet. 
3. Use 2014 data to create pivot table with "County" as row and "SUM of n" and "SUM of nPBE" as values. 
4. Copy pivot table into new sheet and paste as "values only." 
5. Use division formula to find percent of PBE in each county. In other words, I am dividing number of PBE of each county by the total number of incoming kindergarteners. 
6. Sort the "percentage of PBE" from "Z-A"(in descending order)
7. The chart below illustrates my findings: 

!['Question1','pivotTable'](/Question3.jpg)

**What percent of incoming kindergarteners in each county had PME in 2014?**
1. Use filter tool to show just data for 2014. 
2. Copy data for 2014 into new sheet. 
3. Use 2014 data to create pivot table with "County" as row and "SUM of n" and "SUM of nPME" as values. 
4. Copy pivot table into new sheet and paste as "values only." 
5. Use division formula to find percent of PBE in each county. I am dividing the number of PMEs in each county by the total number incoming kindergarteners to find the percentage. 
6. Sort the "percentage of PME" from "Z-A" (in descending order)
7. The chart below illustrates my findings: 

!['Question1','pivotTable'](/Question4.jpg)

**What is the percent change between 2000 and 2015 for DTP vaccinations in incoming kindergarteners?**
* Please note that percent change could not be calculated for Alpine county because data is only available between 2000 and 2013 for Alpine county.
1. Pivot table. Row as "County." Value as "SUM of nDTP."
2. Use filter to isolate this pivot table for 2000. Copy this data into new sheet as "values only."
3. Use filter on pivot table again to isolate data for 2015. Copy "nDTP" for 2015 into the new sheet. 
4. Use percent change formula which is (New-Old/Old X 100) to find percent change. 
5. Sort percent change of DTP from "Z-A"(in descending order). 
6. The chart below illustrates my findings:

!['Question1','pivotTable'](/Question5fixed.jpg)

**What is the percent change between 2000 and 2013 for DTP vaccinations in Alpine County for incoming kindergarteners?**
1. Pivot table. Row as "County." Value as "SUM of nDTP."
2. Use filter to isolate this pivot table for just Alpine County.
3. Then use another filter to just show the year 2000. Copy this data into new sheet as "values only."
4. Use filter on pivot table again to isolate data for just 2013. Copy "nDTP" for 2013 into the new sheet. 
5. Use percent change formulato find percent change. 
6. Sort "percent change of DTP" from "Z-A"(in descending order). 
7. The chart below illustrates my findings:

!['Question1','pivotTable'](/Question6.jpg)

**According to the data that outlines pertussis cases by counties in California, 2014 had the most number of cases.**
* To examine if there is a relationship between the number of cases and vaccinations trends, I used VLOOKUP to join the data for pertussis cases in 2014 with an 2014 version of the kindergarten data. Please note that there was no data available for Alpine County in 2014 which I replaced as "n/a" as placeholders.
1. Use pivot table and input "County" as rows. And the following as values as SUM of: "n", "nDTP","nPME", and "nPBE."
2. Then I used "year" filter to just show data for 2014. 
3. I copied the pivot table as "plain text" into a new sheet. 
4. Next, I created two new columds called, "Pertussis Cases" and "Pertussis Rates."
5. Finally, I used VLOOKUP to join 2014 pertussis case data. 
6. The joined 2014 data is shown below:

!['Question1','pivotTable'](/Question7.jpg)

**I'm interested in analyzing DTP vaccination rates, PME rates, and PBE rates for kindergarteners in comparison to the pertussis rates at large in 2014. I'm adding to the 2014 dataset I just joined above.**  
* Calculating DTP vaccination rates for incoming kindergarteners by county. 
1. Add new column titled, "Rate of vaccination of DTP for incoming kindergarteners(per 100,000)."
2. For each county, divide nDTP by n(the total number of students). Then, multiply by 100,000. 
* Calculating PME rates for incoming kindergarteners by county. 
1. Add new column titled, "Rate of PME for incoming kindergarteners (per 100,000)"
2. For each county, divide nPME by n. Then, multiply by 100,000.  
* Calculating PBE rates for incoming kindergarteners by county. 
1. Add new column titled, "Rate of PBE for in coming kindergarteners(per 100,000)"
2. For each county, divide nPBE by n. Then, multiply by 100,000. 

**_The updated 2014 data is shown below:_** </br>
_Please note that data from StudentData.csv is filled in red, data from pertusisRates2010_2015.csv is filled in orange, and data I calculated is filled in yellow._
!['Question1','pivotTable'](/Question8fixed.jpg)


## Story Pitch</br> 
In 2013, the rate for pertussis cases were 6.64 per 100,000 people in California. In 2014, the rate for pertussis cases was 28.35 per 100,000 people in California. I will be exploring this rise of pertussis cases in 2014 by writing a story that explores this occurence. First, I begin my story by going over the overarching facts and trends about pertussis in 2014. This [2014 article](https://www.cdc.gov/mmwr/preview/mmwrhtml/mm6348a2.htm) published by the Center for Disease Control and Prevention declared a pertussis epidemic in California. This will be used to discuss the pertussis epidemic at large. To make sense of the importance of giving your children the DTP vaccine from a medical professional, I will interview Dr.Tomás Aragón, the director of California Department of Public Health. Dr. Aragón is also an assistant adjunct professor at UC Berkeley. He can be reached through his email at: aragon@berkeley.edu. 

Then the story will focus on Humboldt county as the case study for how refusing to vaccinate children can lead to outbreak in the county at large. By merging "StudentData.csv" and "pertusisRates2010_2015.csv" for the year 2014 and then calculating the rates per 100,000 people for PME and PBE of incoming kindergarten students(from StudentData.csv)-- I intended to find if high PME and PBE rates in incoming kindergarteners had an impact on pertussis infection rates at large in the county. I found that the data suggested a relationship between high PME and PBE rates in incoming kindergarteners and pertussis rates at large in 2014. The table below shows relevent findings:

**The counties with the highest pertussis rates(in descending order):**
County | Pertussis Rates(per 100,000)
-------| -----------
Sonoma County | 142.18  
Humboldt County|103.84
Marin County| 103.17
Napa County|97.77
Yolo County|70.32

**The counties with the highest nPME for incoming kindergarteners(in descending order):**
County | nPME per 100,000
-------| -----------
Kern County| 580  
Butte County|554
Nevada County| 477
Placer Couny|401
Humboldt County|392

**The counties with the highest nPBE for incoming kindergartners(in descending order):**
County | nPBE per 100,000
-------| -----------
Nevada County| 21,360  
Mariposa County| 14,650
Mono County| 11,029
Humoldt Couny| 10,327
Santa Cruz County| 9,011

As the data illustrates, among the highest PME and PBE rates for incoming kindergarten students was Humboldt County, which was also the county with the second highest number of pertussis cases in 2014. </br>
To gain better insight into the high number of PME and PBE in Humboldt County, I will interview Dr. Chris Hartley, the superintendent of schools for Humboldt County. He can be reached at superintendent@hcoe.org. I would make sure to also ask him the qualifications of PME and PBE and whether he believes in the validity of these exemptions.</br>
Moreover, the data also suggests that there are significantly more personal belief exemptions than permanenet medical exemptions. Personal belief exemptions could be rooted in conspiratorial beliefs as such narratives that doubt the safety of vaccines like DTP have been circulating. After interviewing the superintendent of Humboldt County about PME and PBE. It would be beneficial to report the psychology of believing in such conspiracy theories. There is a [2017 peer-reviewed journal article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5724570/) published in _Current Directions in Psychological Science_. I can use this article to inform readers on why one may find conspiracy theories appealing because understanding the psychology behind it may empower people to stay away from such fallacies. 

## Data Visualization 
For the data visualization, I created a chloropleth map that shows the pertussis rate per 100,000 people by each county in California for 2014. 
The [live chloropleth map](https://www.datawrapper.de/_/3TlCd/) can be seen by clicking the link.
The screenshot is included below:
!['Question1','pivotTable'](/pertussisratemap.jpg)
