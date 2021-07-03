# Kickstarter_Challenge
Analysis of Louise’s play Fever fundraising goal review with respect to how different campaigns range performed at different ranges and months in relation to their launch dates and their funding goal.
# Kickstarting with Excel

## Overview of Project: 

Louise’s fundraising goal was reviewed with respect to how different campaigns fared in relation to their launch dates and their 
funding goal.Visual information of campaign outcomes based on their launch dates and their funding goals 
were presented to support required information for effecective reporting.
			
### Purpose : 	
This analysis was provided based on Louise’s fundraising goal in a short amount of time.
 
## Analysis and Challenges :
Datas were analyzed wiith outcomes based on launch date chart and outcomes based on goals Chart.
Some of the challenges encountered includes the conversion of "launched_at" numbers in column "J" to date. 
This was achieved using the the excel formula ((("P"/60)/60)/24)+DATE(1970,1,1) for the conversion 
of numbers to date in column "P" in a new sheet.

### Analysis of Outcomes Based on Launch Date : 
Pivot table was created from the KickStarter worksheet,  the pivot table was placed
Sheet was labelled "Theater Outcomes by Launch Date.".Pivot table was
filtred based on "Parent Category" and "Years." with the appropriate table 
fileds in the columns, rows, and value sections. Column labels were 
filtered to  show only "successful," "failed," and "canceled."
Using  Filter, the "Parent Category"  showed only the data for "theater." 
						
![Plot 1](https://github.com/Adegbenga1/Kickstarter_Challenge/blob/main/Theater%20Outcomes%20Lauch%20dates.png?raw=true)	
						
### Analysis of Outcomes Based on Goals :

Analysis of  Outcomes Based on Goals based was achieved by creating column to hold Goal,
Number Successful,Number Failed,Number Canceled,Total Projects,Percentage Successful,Percentage Failed
and Percentage Canceled, Dollar amount ranges were created in Goal colums so tha projects could be 
grouped based on their goal amount. 

COUNTIFS() functions (examples below )were used to populate the "Number Successful," "Number Failed," 
and "Number Canceled" columns by filtering on the Kickstarter "outcome" column, on the "goal" 
amount column using the ranges created.

COUNTIFS(' Kickstarter_Challenge'!$D$2:$D$4065,"<1000",' Kickstarter_Challenge'!$F$2:$F$4065,"successful")
COUNTIFS(' Kickstarter_Challenge'!$D$2:$D$4065,">=1000",' Kickstarter_Challenge'!$D$2:$D$4065,"<="& "4999",' Kickstarter_Challenge'!$F$2:$F$4065,"successful")
					  
Subsequently , the sum() fuction was used to to populate the "Total Projects" column 
with the number of successful, failed, and canceled projects for each row. 
The percentage of successful, failed, and canceled projects for each row was calculated 
and a line chart created. Analysis of  Outcomes Based on Goals based was achieved by creating column to hold Goal,
					
### Challenges and Difficulties Encountered :

Based on previous lectures and on-hand practice, the challenges encountered were
not too difficult to handle. Creating a counif() was a challenge but not difficult.

## Results :

Results showed that Outcome based on launch dates were very successful in May and June despite the 
fact that we had approximately 50% fails when compared with failed outcomes.
61% of the total outcomes showed successful with 36% failed and 3% cancelled.

Outcomes based on goals were significant for ranges between $1000 - $4999 and Less than 1000 . The percentage success  were
66% and 71% respectively.
There was zero number of successful outcomes for goal range between $35000 - $39999 culminating to 76% of failed outcomes for this range.
The most successful ranges are Less than 1000,$1000 - $4999 ,$5000 - $9999 and $10000 - $14999

# What are two conclusions you can draw about the Outcomes based on Launch Date? 
-	 Launching will be more successful between MAy and August . However, the month 
 	of May shows more shows significant potential succes for launch dates

# What can you conclude about the Outcomes based on Goals? 
- 	Target goals should be between less than $1000 to $14999. in order to achieve anexceellent results

# What are some limitations of this dataset? 
- 	Data types conversion is one of the limitations 

# What are some other possible tables and/or graphs that we could create? 
- 	Pie charts , and Box and whiskers charts could sfuther support analysis and visualizations
- 	



