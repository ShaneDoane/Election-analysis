## Overview of Election Audit
The purpose of this project was to automate the summarizing of election results using Python. The summary includes the following for each county: voter turnout, portion of total election vote, and which county had the largest turnout. For each candidte: vote count and percent of total votes. This script also determines the winning candidate based on popular vote.

## Election Audit Results
Results are shown in the following image of the printed txt file that this script will produce.

![image](https://github.com/ShaneDoane/Election-analysis/blob/main/Resources/Election_Results.png)

## Summary
This script can be used for auditing future elections of any type. The only variables needed are: unique ballot ID, County (or other geographic segment) and Candidate. One recommendation is to change the county-oriented lists and dicts to state, or municipal districts, etc. based on the context of the election. Image of example county-oriented lists below.

<img width="442" alt="image" src="https://user-images.githubusercontent.com/93338132/149597790-09e7a774-1c68-4102-b894-8fc668d5db4d.png">

 The other modification to make would be to potentially modify this if statement to allow declare a winner if the candidate receives a true majority (>50%) of votes. That could be possibly done by changing Line 137 "if (votes > winning_count) and (vote_percentage > winning_percentage):" to "if (votes >= 0.5 * total_votes) and (vote_percentage >= 0.5):
 
 <img width="630" alt="image" src="https://user-images.githubusercontent.com/93338132/149597937-9fb97205-03ad-401a-9338-00ea36af0b65.png">
