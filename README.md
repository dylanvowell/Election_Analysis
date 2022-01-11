# Election Audit Overview
Counting votes in elections used to be a tedious and completeliy manual process. With the advent of digital technology, we are now able to save large amounts of time by automating the process with the trade-off of some time invested up-front. Python is incredibly good at automating boring, tedious tasks and that's why it was chosen for this project. I used Python to count the total votes, assign the votes to their appropriate candidate and county, determine who the winner was, and finally display all of the resuults into a text file for ease of access. 
#Election Audit Results
- 369,711 votes were cast
- Votes for each county from txt file
  > County Votes:
  > - Jefferson: 10.5% (38,855)
  > - Denver: 82.8% (306,055)
  > - Arapahoe: 6.7% (24,801)
- Denver had the most votes out of each county
- Votes for each candidate from txt file
  > - Charles Casper Stockham: 23.0% (85,213)
  > - Diana DeGette: 73.8% (272,892)
  > - Raymon Anthony Doane: 3.1% (11,606)
- Winning Candidate Breakdown from txt file
  > - Winner: Diana DeGette
  > - Winning Vote Count: 272,892
  > - Winning Percentage: 73.8%
# Election-Audit Summary
This python script is not only compatible with this particular election. Most of the lines of code can be re-used as long as the .csv file with the votes are available, and specific variables are changed around to accomodate for the type of election being audited (city, county, state, national). Below are some of the areas to change:
```
# 1: Create a county list and county votes dictionary.
county_list= []
county_dict={}
```
Above, you can change the county variables to represent districts, cities, states, etc. 
```
# 2: Track the largest county and county voter turnout.
largest_turnout=""
largest_count=0
```
Instead of counting the largest turnout, this section can be repurposed to show electoral college votes if you were using this script for a national election. 
