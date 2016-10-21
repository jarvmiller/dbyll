---
layout: post
title: NBA Overtime Games
category: Data
tags: r
---

I was recently curious about how big the home advantage affects overtime games in the NBA. 

I went to basketball-reference.com and used rvest to scrape some of the data and then cleaned it using stringr, dplyr, and reshape2. I then found the percentage that each 
team wins in OT games and plotted that. I didn’t merge or delete defunct team since those teams either got relocated (due to low 
attendance) or revamped which probably played a big part in its success. Thus, there are a number of teams that aren’t established 
today. I could improve this by penalizing teams who only played in a few OT in comparison to older teams (e.g. Pelicans vs Lakers or 
Celtics)… I probably will later on. Also, ggrepel is so lovely. Grateful to have something make nice labels for plotting.
![alt text](https://raw.githubusercontent.com/jarvmiller/jarvmillerr.github.io/master/images/nba.ot.team.png)

I also did a couple classic ‘home vs away’ plots. It shows the per-year percentage of home court victory in OT games. Overall, nothing too strange besides the year 1956. Wonder what
happened there. Oh yeah, home team won 52.8% of all games from 1949-2015. Might be a tad bit higher if you don’t count 1956. 
![alt text](https://raw.githubusercontent.com/jarvmiller/jarvmillerr.github.io/master/images/nba.ot.line.png)
