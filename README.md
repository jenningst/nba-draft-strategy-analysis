<p align='center'>
  <img width="600" src='https://github.com/jenningst/nba-draft-strategy-analysis/blob/main/images/tj-dragotta-Gl0jBJJTDWs-unsplash.jpg' alt='Basketball'>
</p>
<p align='center'>
  Photo by <a href="https://unsplash.com/@tjdragotta?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">TJ Dragotta</a> on <a href="https://unsplash.com/s/photos/basketball?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
</p>

# NBA Draft Strategy Cluster Analysis

In this project, we attempt to answer the following question: is there a significant difference in categories won, based on drafting strategies that selects either guards or "big-men" in the later rounds?

## Motivation

For the purposes of this analysis, we will be using the data which corresponds to a 9-category fantasy basketball league. In this league format, league players compete against 9 categories – field goal percentage, free throw percentage, total three pointers, total rebounds, total assists, total steals, total blocks, total turnovers, and total points. League participants mock draft NBA players to optimize the number of categories they win each week when competing against a fellow league participant.

## Method and Results 

We know that players aren’t always assigned a singular position: they can often play multiple positions (i.e., they have utility in more than one position). For purposes of this analysis, we will consolidate player positions into the primary five – point guard (PG), shooting guard (SG), small forward (SF), power forward (PF), and center (C) – by reassigning them to the position the player plays the most.

From collected summary statistics, we notice zero values in all the categories. If we were truly drafting players for a fantasy league, we avoid players with low usage (e.g., low minutes played or low games played), since there will be a direct correlation between minutes played/games played and the category statistics. For purposes of this analysis, we remove players with minutes played less than the mean minutes played for the entire league. After removing players with low minutes played, we notice there are still sufficient remaining players for 10-player rosters for a 14-team fantasy league.

We then run an analysis of the clustering model to determine the optimal number of clusters. This analysis triangulates the optimal number of clusters using three methods – elbow method, silhouette method, and gap statistic.

<p align='center'>
  <img width='600' src='https://github.com/jenningst/nba-draft-strategy-analysis/blob/main/plots/elbow.png'>
</p>

<p align='center'>
  <img width='600' src='https://github.com/jenningst/nba-draft-strategy-analysis/blob/main/plots/silhouette.png'>
</p>

<p align='center'>
  <img width='600' src='https://github.com/jenningst/nba-draft-strategy-analysis/blob/main/plots/gap.png'>
</p>

Now that we have clusters and...


## Project Members
- Romith Challa
- Carl Ausmees
- Troy Jennings (https://github.com/jenningst)
