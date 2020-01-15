# US_Election
# Author: YK

Objective
●	Download the 2016 presidential primary results 
●	Parse the content and structure it into a dataframe
Using BQPlot, create an interactive visualization of the results for each state and each party’s primary outcome.
The visualization should look similar to the maps in this NYT article:
https://www.nytimes.com/elections/2016/national-results-map


Prerequisites

●	BeautifulSoup4: this should already be packaged in the Anaconda3 distribution or else do:
conda install beautifulsoup4 

Data Description
The Politico website 
●	www.politico.com/mapdata-2016/2016-election/primary/results/map/president/ 

contains all the information of the 2016 presidential primaries, including party, primary type (caucus / primary), date, 
candidates running in each primary, votes and vote% won, as well as delegates won.

Tasks:

Scrape and organize the Data:

Using BeautifulSoup scrape the state level for both parties and output the results in a df_results DataFrame indexed by
●	electiontype: one of ['Caucus', 'Primary']
●	state: state of the election
●	date: date at which the election took place
●	party: one of ['GOP', 'DEM']
and containing the following columns
●	candidate: candidate name
●	votes: votes the candidate won
●	%votes: %votes the candidate won
●	delegates: delegates that candidate won 

Visualize the data using BQPlot

Using BQPlot, create an interactive visualization of the results for each state and each party’s primary outcome. The visualization should look similar to the maps in this NYT article and should have the following features:
●	There should be one visualization for the GOP primaries and another for the DEM primaries.
●	In each such visualization, the state-level map should have each state colored by the color of the winner for that state - use similar colors as those in the NYT article.
●	When scrolling over each state, a hover popup should appear which shows the total number of votes each candidate received at the state level. Note that the NYT visualization does the same for each congressional district. You will only need to do this for each state on aggregate.
		 
