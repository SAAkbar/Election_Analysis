# Election_Analysis
## Overview of Election Audit
An election commission from Colorado requested an audit for a US congressional precinct’s election. The commission asked for all the votes to be counted, the number and percentage of votes for each candidate and to find the winner of the election. Later, the commission also requested additional info based of the counties, mainly the voter turnout and percentage of votes from each county and the county that had the highest turnout. Counting votes one by one can be tedious but since the votes were sent in a CSV file, the logical route was to streamline the counting of the votes, for this case Python was used.  
## Election-Audit Results
•	Total votes: 369, 711

•	Number of votes and the percentage of total votes for each county:

        o	Jefferson: 38, 855 (10.5%)
  
        o	Denver: 306, 055 (82.8%)
  
        o	Arapahoe: 24, 801 (6.7%)
  
•	County with the largest turnout: Denver (306, 055)

•	Number of votes and the percentage of the total votes each candidate:

        o	Charles Casper Stockham: 85, 213 (23.0%)

        o	Diana DeGette: 272, 832 (73.8%)

        o	Raymon Anthony Doane: 11, 606 (3.1%)

•	Winning Candidate: Diana DeGette with 272, 832 votes, 73.8% of the total vote count

### Output of Results from Terminal

![image](https://user-images.githubusercontent.com/76131315/104863132-2d9d7580-5903-11eb-84ef-6b7758c2173d.png)

## Election-Audit Summary
The code was able to give us the results seen in the section above, but this code is also able to help for other elections. One way it can help is if the commission wanted to audit another precinct all they would have to do is to add the CSV file for the new precinct to the resources folder and change the name to the new CSV file in line 9 (Line 9 is seen below). So, instead of “elections_results.csv” it will be the new CSV file name, ie “new_elections.csv” of course this is under the assumptions that the new file is formatted the same as the old one in which there are ballot Id, county and candidate in that order.

![image](https://user-images.githubusercontent.com/76131315/104862707-d5b23f00-5901-11eb-87cc-b97af340b3c6.png)

Another way that this code can help the commission with other elections is if they would like to audit elections that are bigger or smaller in scale, for example if they want to audit the national elections. For this election, they would have state as a header which they would probably be interested in knowing the number of votes, their percentages and which state had the largest turnout. To make the code work for this, the first thing they have to do to the code is change the CSV file as talked about above, after the short and easy thing to do is to just change line 50(see below) on the code to count the state rows, for example if the states are under 5th header in the CSV then the number is 4, just like in our case the county was under the 2nd header so we put a 1 there, if you do this you would also have to change like 88 (see below) from County Votes to State Votes and line 114 (see below) from Largest County Turnout to Largest State Turnout. This would make the out come say state instead of counties and this way is only good if they only want the results and will never look at the code again. The long way to do this is to do what’s above but also to change all the county variables to say state instead of county, this is better if they want to pass this code to other colleges so it is easier to follower along and this way it would make sense.  

![image](https://user-images.githubusercontent.com/76131315/104862968-a6e89880-5902-11eb-92d4-ce85b0212ddb.png)

![image](https://user-images.githubusercontent.com/76131315/104862827-29248d00-5902-11eb-9681-0dae9a37cfa2.png)

![image](https://user-images.githubusercontent.com/76131315/104862871-4fe2c380-5902-11eb-89de-5d27cbef9dba.png)
