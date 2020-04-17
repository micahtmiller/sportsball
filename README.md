# Sportsball Exercise

Spend as little or as much time on this as you'd like.  It is an opportunity to demonstrate your skills without the stress of an interview.  If you cannot spend as much time as you'd like on this, that is OK.  Just leave the details in a TODO file listing the work you'd like to complete and how you intended to proceed.

If you have any questions, please reach out to the interviewer by email.

## Scenario

You have just joined a DevOps team. This team lives by DevOps principles and you want to let them know you mean business! This particular team is developing a product that is deployed in a Google Cloud Project.

This sprint, the team has been asked to write an application that will be used to provide information about baseball player statistics.

You may need to make some assumptions, that's OK, just document what they are and move on.

The team loves innovation, so you can use whatever languages and technologies you like to complete this. Approach this problem as if your code will go to production. Whilst we don’t expect the code to be perfect, we are not looking for a hacked together script.

Your solution should offer the rest of the team a way to trigger the program and return the results.

When you submit your solution, please provide any special setup instructions.

## Assumptions

All requests are based on data in the hitting file. Future requests will require data from a pitching file as well.  Consider this in the design.

## Requirements

Use the provided data to calculate the following results:
* Most improved batting average (hits/at-bats) from 2009-2010
    * Only include players with at least 200 at-bats
* Slugging percentage for all players on the Oakland A's (teamID=OAK) in 2007
* Who was the AL and NL triple crown winner for 2011 and 2012
    * If no one won the crown, output "No winner"

## Formulas

* Batting average = hits / at-bats
* Slugging percentage = ((Hits - doubles - triples - home runs) + (2 * doubles) + (3 * triples) + (4 * home runs)) / at-bats
* Triple crown winner
    * The player that had the highest batting average AND the most home runs AND the most RBI in their league.
    * This is unusual, but it happened in 2012
    * Player must have at least 400 at-bats

## Data

* Batting-07-12.csv - contains all batting statistics from 2007-2012
* Columns
     * AB - at-bats
     * H - hits
     * 2B - doubles
     * 3B - triples
     * HR - home runs
     * RBI - runs batted in

* Master-small.csv - contains the demographic data for all baseball players in history through 2012