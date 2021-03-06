# Election_Analysis

## Project Overview
The Coloado Board of Elections provided the election results of a recent local congressional election in a CSV format.  This projects is to review and summarize the election results to be published.  There were two steps to the analysis.  The first was during the project where we analyzed the candidates and their vote results.  The second was covered in the challenge which focused on summarizing county results (see below Challenge section for further information).  The output from this review summarizes the election results by providing the following data points:
 - total votes collected 
 - the candidates 
 - each candidates individual results (total votes and % of votes)
 - the final winner of the election

## Resources
 - Data Source: election_results.csv
 - Software: Python 3.6.1 Visual Studio Code, 1.38.1

## Summary
The analysis of the election data shows that:
 - 369,711 votes were cast
 - There were three candidate with the following results
   - Charles Casper Stockham: 23.0% of the vote with 85,213 votes
   - Diana DeGette: 73.8% of the vote with 272,892 votes
   - Raymon Anthony Doane: 3.1% of the votes with 11,606 votes
 - The winner of the election was
    - Diana DeGette with 272,892 votes or 73.8% of all votes
 - see below Challenge Summary for County Results

## Challenge Overview
The challenge requested additional information regarding the prior election analysis.  The primary purpose of the challenge was to add county results, specifically the count of votes by county and to identify the county with the largest number of votes.   

## Challenge Summary
The results of the challenge show that:
 - Denver county had the largest voter turnout with 306,055 votes (82.8% of the total votes)
 - Jefferson county had the second largest voter turnout with 38,855 votes (10.5% of the total votes)
 - Arapahoe had the least voter turnout at 24,801 votes (6.7% of the total votes)

## Election Audit Summary
I would recommend utilizing the code created in this analysis in other elections across the state of colorado.  For example:
 - Other precincts could use the code exactly as is for their congressional candidate elections.  Other precincts could either make certain their file naming convention matches that which is in this code or modify the code to fit their naming conventions.  The line item code that needs to be verified :
   line 9 -  `file_to_load = os.path.join("Resources", "election_results.csv")` 
   line 11 -  `file_to_save = os.path.join("Resources", "election_analysis.txt")` 
 - This could also be used for US Senator elections in any state.  Each state elects 2 senators, for 6 year terms.  In this case you don't need to change anything to the code, your source file will just be larger.  Typically not both senate seats are open at one time for states so you will only need to find the candidate with the most popular vote.  You could remove the county portion of the code since the entire population votes for a Senator unless you would like county analytics in your results, which county voted the most and for which candidate.
   
