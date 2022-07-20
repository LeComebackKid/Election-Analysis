# Election-Analysis
---
# Election AuditAnalysis
J. Demone                                                                
DA: Module 3 (July 20, 2022)

## Section 1: Overview
  The votes of the Colorado Precinct’s election have all been cast. It is time to gather the results, but can they be trusted? Who can be trusted to count them? An analysis of the vote will ideally help avoid human error when calculating these results. The last thing that any State needs is non-confidence in their vote count. It could, therefore, be helpful to automate the tabulation of the Colorado Precinct Election using a computer generated system, such as Python.


  Tom and Seth, who are employees of the Colorado Board of Elections Commission, are hoping for some assistance with tabulating the results. Given the large volume of data (i.e., candidates, votes collected, counties) collected, they have set a goal to use Python to generate a code to read and organize the results. Using Python will significantly decrease the amount of time it would take to tabulate the results of this election. 


#### Goals:
  Our goal is to assist Tom and Seth were given some additional assignments. They have been asked to calculate the  total number of votes, the votes received for each candidate and the percentage received. The candidates in this riding include: Diana Degette, Raymon Doane and Charles Casper Stockham. A fourth candidate, Spongebob Squarepants, has dropped out due to some shocking tweets that surfaced last month, and his name was removed from the ballot. 
In addition, the commission has requested information regarding the voter turnout for each population. The counties of focus are Arapahoe, Denver and Jefferson. The information collected includes the total votes for each county and the percentage of votes for each, as well. The success of this analysis is desirable as it could lead to further studies of election results using code. 


## Section 2: Election-Audit Results

  The following outcomes were tabulated in the Colorado Precinct Election Summary: 
        * The total amount of votes were calculated for each county and candidate by identifying each name in a .csv    file of the election results and adding a point for each vote cast
        * The percentage of votes were calculated by finding the total number of votes cast for each candidate or county and dividing that number by the total amount of votes
        *  The total total amount of votes was 369,711
        
        #### Candidates:
        * Of the three candidates, Diana Degette, came out the winner with greatest number of votes, 272,892
        * Ms. Degette received just under ¾ of the total votes, compared to the ¼ of combined votes for Mr. Stockhamn and Mr. Doane
        * Mr. Stochhamn was the second favourite candidate, receiving just under a quarter of the total vote
        * Mr. Doane received only three percent of the votes
           * He announced that he will be stepping down from his party imminently
           * The total votes (and percentage of the total) for each candidate is as follows:
        * Diana DeGette received 272,892 votes  (73.8% of the total vote)
        * Charles Casper Stockhamn received 85,213 votes (23.0% of the total vote
        * Raymon Anthony Doane received 11,606 votes (3.1% of the total vote)
        
        #### Counties :
           * Of the three counties, a significant bulk of the votes were cast in Denver, covering over eighty-percent of the total vote. 
           * The total votes (and percentage of the total) for each county was as follows:
              * Denver - 306,055 votes cast (82.8% of the total vote)
              * Jefferson -  38,855 votes cast (10.5% of the total vote)
              * Arapahoe - 24,801 votes cast (6.7% of the total vote)


## Section 3: Election-Audit Summary
  The **Python Election-Audit Analysis** has proven to be successful! There are some significant reasons as to why this type of analysis is useful, in addition to why it would be a useful tool for other elections. 

#### Time:
  Aside from generating the desired results, the vote count and summary were all calculated quickly. Most of the time that was put into the analysis was on the coding. However, aside from edits to the code that may come over time, the majority of the coding is already completed for future use.
  This program was able to summarize the results of almost 370,000 votes in a matter of seconds. This would also mean that there would need to be a way for the votes to and voter data to be collected so that it could automatically be stored.   
  Further, given the ongoing allegations of voter fraud and miscounts found in many modern elections, this program will provide a timely and easy alternative to recounting results, if necessary.  

#### Learning/Larger Pools
  Beyond calculating votes, computer generated programs, such as this one, are able to rapidly analyze data. This means that an analysis using code could also provide the election committee and voters with more information about the votes and the voting population. This information could be useful in determining patterns among voters. In the case of this analysis, the location of the vote was used to determine which county had the largest voter turnout. 
This type of information could be helpful with determining cities for campaigns, to set up an adequate amount of voting stations and to avoid lineups at polls. It could also be helpful in targeting cities or counties that do not have much of a voter turnout. 
  With this knowledge in hand, the government can focus on educating or encouraging future voters or perhaps make better access to voting stations. Naturally, this analysis is just a first step and more research will need to be accomplished to arrive at a clearer understanding in each case. 

#### Saving Money and Space
  Elections are disgustingly expensive. “Who cares that not every child has a breakfast to eat, this candidate needs to have an election before their quarterly results come in!” 
  Sound familiar? Using code to automate the results could decrease the amount of bodies required to process an election. It could also decrease the need to rent spaces where votes are calculated or stored. In both cases, you will need less people and space to run this type of analysis. With inflation running so high, who wouldn’t want to save some extra money? 


### Suggestions/Modifications For Future Trials:

#### More Variables = More Learning
  There are an infinite number of directions in which this analysis can proceed for future use. One easy way to benefit from using the analysis as a learning tool would be to include more variables. 
    These days, the saying,  “know your audience”, is truer than ever. Pretty much, on a daily basis, all the information that passes through the general public’s eyes and ears is personally marketed to their unique interests or characteristics. This focus depends on the variables and how they relate. 
  These “variables” are essentially what makes an individual but also what connects that individual with a larger population. Some examples of other focus areas include, age, gender, race, occupation, income, etc. Essentially, if you did not vote for a party in a past election, then that party could use this information to learn about the general public and find a way for their political party to engage their interests for the next election. 
Reorganization Of Coding Script
In order to help with future development of this program, it would be helpful to revisit the organization of the code so that new additional variables could be added. 
In the early stages of the coding, the only variable that was of focus was the winning candidate. As a second measure was added - looking at the county vote turnout - it became increasingly difficult to retrieve the intended output. While the output was still retrievable, some realignment or relocation of the code would make it a bit more logistical. This focus would also be helpful, as it would help identify the areas that need to be mended if the desired results are not met. 
Finally, a new area of focus or measure that is added could hopefully be included in a less complicated format. This may not always be the case, depending on the results that are being achieved. In any case, using f-strings is highly recommended, as they are more time efficient. 
For example, look at the code used below to identify the results for the county vote turnout. Using helpful strings, such as this will help with using time efficiently when creating the program. 
county_results = (f"{county_name}: {county_vote_percentage:.1f}% ({county_votes:,})\n")
       print(county_results)

#### Reliability
One other area to consider is that of reliability. How much of this information collected is actually correct? On one hand, removing people from counting individual ballots could help avoid problems such as human error (intended or unintended). However, using code to count is also questionable. How reliable is the data?
If modern elections have taught the world anything, it is that data can be compromised. Therefore, for this program to be a reliable and trusted tool, there would need to be an element of security that would need to be implemented. It will also need to be conducted in a way so that the general population trusts the results and the integrity of the analysis. This means preventing incidents of “virtual vandalism” or hacking to the data that is stored from these elections is of the utmost importance. In this case, a hard copy of the raw data would also be ideal if the integrity were to be questioned. 
Overall, this tool has proven to be successful when analyzing the data from the Colorado Precinct’s election. Beyond this success, it is also full of potential for larger data pools and further learning or analysis.
