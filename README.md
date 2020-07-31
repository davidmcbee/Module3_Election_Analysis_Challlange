# Module3_Election_Analysis_Challlange
## Overview of Election Audit
My role was to assist a Colorado Board of Elections employee, Tom, in an election audit of the tabulated results for a U.S. congressional precinct in Colorado. Tom’s manager, Seth, wanted to know if there is a way to automate this analysis with Python. If successful, this code will then be used to audit other congressional districts and senatorial as well as local elections.

### Scope
The specific deliverables for this audit were:
1.	The total number of votes cast
2.	The voter turnout for each county
3.	The percentage of votes from each county out of the total count
4.	The county with the highest turnout
5.	The percentage of votes for each candidate
6.	The total number of votes for each candidate
7.	The winner of the election based on the popular vote

### Voting Methods
There are three voting methods:
1.	Mail-In Ballot
2.	Punch Cards
3.	Direct Recording Electronic
The votes from these three methods were sent to the central office and tabulated.

### Vote Information
The information from the central office, for this analysis, was provided in a CSV file containing three columns and 369712 rows, including a header row. The three columns are Ballot ID, County and Candidate.
The product from this analysis is to provide a vote count report to certify the election results.

## Election-Audit Results
The results from the analysis is available here and shown in table 1
The audit questions and answers to those questions asked are:
![] (https://github.com/davidmcbee/Module3_Election_Analysis_Challlange/blob/master/Challenge_analysis/Results_table.png)


Questions to Answer	Answers
What was the total number of votes cast?	369,711
What was the voter turnout for each county?	Jefferson – 38,855
Denver – 306,055
Arapahoe – 24,801
What was the percentage of votes from each county out of the total count?	Jefferson – 10.5%
Denver – 82.8%
Arapahoe – 6.7%
What county had the highest turnout?	Denver
What was the percentage of votes for each candidate	Charles Casper Stockham – 23.0%
Diana DeGette – 73.8%
Raymon Anthony Doane – 3.1%
What was the total number of votes for each candidate	Charles Casper Stockham – 85,213
Diana DeGette – 272,892
Raymon Anthony Doane – 11,606
Who was the winner of the election based on the popular vote, their vote count and percentage of total votes?	Diana DeGette with 272,892 votes which is 73.8% of the total vote count
Getting to These Results using Python
The python code to conduct this analysis is available here.  There were a number of steps that needed to be coded to arrive at the results shown above. These are:
1.	Import two python libraries to be used in the code. Provide a path to the provided CSV file and create a path to the text file which holds the results. Additionally, a number of variables, lists and dictionaries were declared and used throughout the code. See lines 1 – 25.
2.	Loop through each row and count the candidate votes. See lines 26 – 57
3.	Loop through the counties and count the votes for each county. See lines 58 – 71
4.	Print the total votes to the terminal and save the total votes to the election_analysis text file. See lines 73 – 86
5.	Calculate the county vote percentages and print the county, the county vote percentages and county votes. Print that and save it to the  election_analysis text file. See lines 88 – 101.
6.	Calculate, print and save to the election_analysis text file, the largest county turnout. Lines 103 – 117
7.	Calculate and print the candidate votes, vote percentage and print them. – Lines 119 – 131
8.	Determine the winning candidate, winning count, winning vote percentage. Print and save that. Lines 133 - 152
9.	Election-Audit Summary
The hope is that many will find this analysis useful. It can be used in its current form regardless of number of candidates, voters or counties. If the consensus is that this would be useful in the future, then there are a few other items of information I propose we add to this analysis to make it even more useful.
Specifically, if the data is available, or can be collected for city votes, political party and voting method used, we could:
1.	Determine the vote count and percentage by the city within each count. This would break the data down to provide more granularity
2.	Comparing the political party to who the vote was cast for could reveal political party strength. Further it could provide insight into how independent party voters are trending.
3.	Understanding how many people cast their vote from among the three voting methods, Mail-In Ballot, Punch Cards or Direct Recording Electronic would provide insight into areas for investment; provide better customer service.
