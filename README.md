# Election_Analysis_Challenge
Repository for Election_Analysis Challenge
 
 ## Overview of Election Audit
 A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election

1. Calculate the total number of votes cast
2. Get a complete list of candidates who received votes
3. Calculate the total number of votes each candidate received
4. Calculate the percentage of votes each candidate won
5. Determine the winner of the election based on popular vote
6. Calculate the voter turnout for each county
7. Calculate the percentage of votes from each county out of the total count
8. Determine the county with the highest turnout

## Resources
- Data Source: election_results.csv
- Software: Python 3.6.1, Visual Studio Code, 1.38.1

## Election-Audit Results
The analysis of the election shows that:
- There were 369,711 votes case in the election.  
     *this was determined using a `for` loop to get the total number of rows in the file and then adding the rows together to get a total vote calculation `total_votes += 1`
- The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were:
  - Charles Casper Stockham received 23.0% of the vote and 85,213 votes
  - Diana DeGette received 73.8% of the vote and 272,892 votes
  - Raymon Anthony Doane received 3.1% of the vote and 11,606 votes
- The winner of the election was:
  - Winner: Diana DeGette
  - Winning Vote Count: 272,892
  - Winning Percentage: 73.8%
- The voter turnout for each county was: 
  - Jefferson county had 38,855 votes, which was 10.5% of total votes 
  - Denver county had 306,055 votes, which was 82.8% of total votes
  - Arapahoe county had 24,801 votes, which was 6.7% of total votes 
    * The percentage was calculated by dividing the number of votes from the county by the total number of votes
     `countyVote_percentage = float(countyVotes) / float(total_votes) * 100
        county_results = (
            f"{county_name}: {countyVote_percentage:.1f}% ({countyVotes:,})\n")`
- The County with the Largest Turnout was Denver county with 82.8% of total votes

## Election-Audit Summary
As shown this script is useful for determining some election results for the three counties listed.  This same script could be use for analysis of similiar data on other (potentially larger) elections.  This script could also be modified to
1. do additional analysis of this data including breakdown of results (winner) by county 
2. provide further breakdown by city or neighborhood (assuming the data was available)
