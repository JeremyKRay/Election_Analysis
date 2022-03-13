# Election Audit

## Election Audit Overview
A Colorado Board of Elections employee has given me the task of completing an election audit of a recent local congressional election.
### Election Audit Purpose

The purpose of this election audit is to analyze the results of a recent local congressional election. The audit includes an analysis that provides the following:

  1. The total number of votes cast.
  2. A complete list of counties that turned in votes.
  3. Total number of votes for each county.
  4. The percentage of votes for each county.
  5. The county that had the largest voter turn out.
  6. A complete list of candidates who received votes.
  7. Total number of votes each candidate won
  8. The percentage of votes each candidate won.
  9. The winner of the election based on popular vote.

## Resources
- Data Source: election_results.csv
- Software: Python 3.6.1, Visual Studio Code, 1.38.1

## Election Audit Results
The analysis of the election show that:
- There were **369,711** votes cast in the election.
- There were three counties represented in the election:
  - County 1: **Jefferson**
  - County 2: **Denver**
  - County 3: **Arapahoe**
- The county results were:
  - County 1, **Jefferson County**, turned in **10.5%** of the vote with **38,855** votes.     
  - County 2, **Denver County**, turned in **82.8%** of the vote with **306,055** votes.
  - County 3, **Arapahoe County**, turned in **6.7%** of the vote with **24,801** votes.
- The county with the largest turn out of voters was:
  - County 2, **Denver**, which turned in **82.8%** of the vote with **306,055** votes. 
- The candidates were:
  - Candidate 1: **Charles Casper Stockham**
  - Candidate 2: **Diana DeGette**
  - Candidate 3: **Raymon Anthony Doane**
- The candidate results were:
  - Candidate 1, **Charles Casper Stockham**, received **23.0%** of the vote and **85,213** number of votes.
  - Candidate 2, **Diana DeGette**, received **73.8%** of the vote and **272,892** number of votes.
  - Candidate 3, **Raymon Anthony Doane**, received **3.1%** of the vote and **11,606** number of votes.
- The winner of the election was:
  - Candidate 1, **Diana DeGette**, who received **73.8%** of the vote and **272,892** number of votes.

The results of the audit can be printed to the terminal screen or they can be viewed in the attached text file. ![Election_Audit_Results](Analysis/election_analysis.txt).

## Election Audit Summary
The task of completing an election audit of a local congressional election was completed by analyzing a csv file of election data using Python programming language and Visual Studio Code editor software. The file contains nearly 370K records and the code I developed loops through each record, grouping the data by first the county and then the candidate, and calculates the total and percentage for each unique county and candidate. It does this quick and efficiently. Because of this, the election commission should know that this same code can be used to conduct audits on future elections. If future elections simply contain more or less candidates or cover more or less counties, the code would not need to be changed at all. If additional data is provided and the commission would like to know additional information, the script could be modified to complete varying types of audits. For example:
  1. If city or district data is added to the csv file, the code for analyzing the file based on county could be copied and just rewritten for district and city. New variables, definition, and list would need to be created, but the code could remain the same but replacing "county" with "city" or "district". 
  2. If demographic data were added to the csv file, such as sex or race, this could also be anaylzed using this code with some modification. If you simply just want to know numbers and percentages of the various demographic parameters, it would simply needed to be added in the same way as adding a "district" or "city" column to be counted. It gets to be a little more complicated if you want to analyze this data across the group of counties or across the group of candidates. This would require additional conditions added to the candidate and/or county 'for' loops. It may even require a nested loop. The idea is to group by candidate or county first and then group by demographic within each county or candidate. So, I think the "demographic" loop would need to be created outside the existing "county" and/or "candidate" loop so that the latter is counted first and then the demographics. 

The full code can be viewed by clicking the following link. ![Election Analysis Python Code](PyPoll_Challenge.py).
